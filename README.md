# Learning IDP: Test-Driven Development

This repository focuses on Test-Driven Development (TDD) practices specifically for Internal Development Platform (IDP) infrastructure and automation code using Python and Azure SDK.

## 🎯 Learning Objectives

By working through this repository, you will:

1. Master TDD principles for infrastructure code
1. Write effective unit tests for Azure SDK operations
1. Implement integration tests with Azure resources
1. Create reusable test fixtures and mocks
1. Set up CI/CD pipelines for automated testing
1. Apply TDD workflow to infrastructure provisioning
1. Understand testing pyramids for platform engineering

## 📚 Prerequisites

- Python 3.11 or higher
- Basic understanding of pytest
- Azure subscription (for integration tests)
- Azure CLI installed (for authentication)
- Git and GitHub account

## 🗂️ Directory Structure

```
learning-idp-test-driven-development/
├── README.md                          # This file
├── REFERENCES.md                      # Links to resources and related repos
├── pyproject.toml                     # Python project configuration
├── requirements.txt                   # Python dependencies
├── requirements-dev.txt               # Development dependencies
├── .python-version                    # Python version for pyenv
├── .gitignore                         # Git ignore patterns
├── pytest.ini                         # Pytest configuration
├── .env.example                       # Environment variables template
│
├── docs/
│   ├── concepts/
│   │   ├── 01-tdd-fundamentals.md
│   │   ├── 02-testing-pyramid.md
│   │   ├── 03-infrastructure-testing.md
│   │   ├── 04-mocking-strategies.md
│   │   └── 05-test-fixtures.md
│   ├── guides/
│   │   ├── getting-started.md
│   │   ├── writing-unit-tests.md
│   │   ├── writing-integration-tests.md
│   │   ├── azure-sdk-testing.md
│   │   └── ci-cd-setup.md
│   └── examples/
│       ├── simple-resource-group.md
│       ├── storage-account.md
│       ├── virtual-network.md
│       └── end-to-end-scenario.md
│
├── src/
│   ├── __init__.py
│   ├── azure_helpers/
│   │   ├── __init__.py
│   │   ├── authentication.py          # Azure authentication utilities
│   │   ├── resource_manager.py        # Resource management base classes
│   │   └── exceptions.py              # Custom exceptions
│   │
│   ├── resource_group/
│   │   ├── __init__.py
│   │   └── manager.py                 # Resource Group operations
│   │
│   ├── storage/
│   │   ├── __init__.py
│   │   └── manager.py                 # Storage Account operations
│   │
│   ├── network/
│   │   ├── __init__.py
│   │   └── manager.py                 # Virtual Network operations
│   │
│   └── compute/
│       ├── __init__.py
│       └── manager.py                 # Compute operations
│
├── tests/
│   ├── __init__.py
│   ├── conftest.py                    # Shared pytest fixtures
│   │
│   ├── unit/
│   │   ├── __init__.py
│   │   ├── conftest.py                # Unit test fixtures
│   │   ├── test_authentication.py
│   │   ├── test_resource_group_manager.py
│   │   ├── test_storage_manager.py
│   │   ├── test_network_manager.py
│   │   └── test_compute_manager.py
│   │
│   ├── integration/
│   │   ├── __init__.py
│   │   ├── conftest.py                # Integration test fixtures
│   │   ├── test_resource_group_integration.py
│   │   ├── test_storage_integration.py
│   │   ├── test_network_integration.py
│   │   └── test_compute_integration.py
│   │
│   ├── e2e/
│   │   ├── __init__.py
│   │   ├── conftest.py                # E2E test fixtures
│   │   └── test_complete_infrastructure.py
│   │
│   └── fixtures/
│       ├── __init__.py
│       ├── azure_credentials.py       # Azure credential fixtures
│       ├── mock_responses.py          # Mock Azure API responses
│       └── test_data.py               # Test data generators
│
├── scripts/
│   ├── setup_azure_test_env.sh       # Setup Azure test environment
│   ├── cleanup_azure_test_env.sh     # Cleanup test resources
│   └── run_tests.sh                  # Run test suites
│
├── .github/
│   └── workflows/
│       ├── unit-tests.yml            # Unit tests CI
│       ├── integration-tests.yml     # Integration tests CI
│       └── e2e-tests.yml             # E2E tests CI
│
└── examples/
    ├── 01_simple_resource_group/
    │   ├── test_first.py             # Your first TDD test
    │   └── implementation.py         # Implementation after test
    │
    ├── 02_storage_account/
    │   ├── test_storage.py
    │   └── storage_manager.py
    │
    ├── 03_virtual_network/
    │   ├── test_network.py
    │   └── network_manager.py
    │
    └── 04_complete_stack/
        ├── test_stack.py
        └── stack_manager.py
```

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/vanHeemstraSystems/learning-idp-test-driven-development.git
cd learning-idp-test-driven-development
```

### 2. Set Up Python Environment

```bash
# Create virtual environment
python3 -m venv venv

# Activate virtual environment
# On Linux/MacOS:
source venv/bin/activate
# On Windows:
# venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
pip install -r requirements-dev.txt
```

### 3. Configure Azure Authentication

```bash
# Copy environment template
cp .env.example .env

# Edit .env with your Azure credentials
# Or use Azure CLI authentication:
az login
```

### 4. Run Your First Test

```bash
# Run all tests
pytest

# Run only unit tests
pytest tests/unit/

# Run with coverage
pytest --cov=src --cov-report=html

# Run with verbose output
pytest -v
```

## 📖 Learning Path

Follow this recommended sequence:

### Week 1: TDD Fundamentals

1. Read `docs/concepts/01-tdd-fundamentals.md`
1. Complete `examples/01_simple_resource_group/`
1. Practice Red-Green-Refactor cycle

### Week 2: Unit Testing Azure SDK

1. Read `docs/guides/writing-unit-tests.md`
1. Study `tests/unit/test_resource_group_manager.py`
1. Implement your own unit tests for Storage Account
1. Learn mocking with `docs/concepts/04-mocking-strategies.md`

### Week 3: Integration Testing

1. Read `docs/guides/writing-integration-tests.md`
1. Set up Azure test environment
1. Complete `examples/02_storage_account/`
1. Run integration tests against real Azure resources

### Week 4: Advanced Testing

1. Study test fixtures in `docs/concepts/05-test-fixtures.md`
1. Implement E2E tests
1. Set up CI/CD pipelines
1. Complete `examples/04_complete_stack/`

## 🧪 Testing Philosophy

### The TDD Cycle

```
1. 🔴 RED: Write a failing test
   - Define what you want to achieve
   - Write the test first
   - Run test (it should fail)

2. 🟢 GREEN: Make it pass
   - Write minimal code to pass the test
   - Don't worry about perfection
   - Run test (it should pass)

3. 🔵 REFACTOR: Improve the code
   - Clean up implementation
   - Optimize if needed
   - Run test (should still pass)
```

### Testing Pyramid for Infrastructure

```
        /\
       /  \
      / E2E \         ← Few, slow, expensive
     /______\
    /        \
   / INTEG.  \       ← Some, medium speed
  /__________\
 /            \
/  UNIT TESTS \     ← Many, fast, cheap
/______________\
```

**Unit Tests (70%)**

- Fast execution
- No external dependencies
- Mock Azure SDK responses
- Test business logic

**Integration Tests (20%)**

- Test against real Azure
- Validate SDK usage
- Check resource creation
- Clean up after tests

**End-to-End Tests (10%)**

- Complete workflows
- Real-world scenarios
- Full stack validation

## 🛠️ Key Dependencies

### Core Testing

- `pytest>=8.0.0` - Testing framework
- `pytest-cov>=4.1.0` - Coverage reporting
- `pytest-mock>=3.12.0` - Mocking utilities
- `pytest-asyncio>=0.23.0` - Async test support

### Azure SDK

- `azure-identity>=1.15.0` - Authentication
- `azure-mgmt-resource>=23.0.0` - Resource management
- `azure-mgmt-storage>=21.0.0` - Storage operations
- `azure-mgmt-network>=25.0.0` - Network operations
- `azure-mgmt-compute>=30.0.0` - Compute operations

### Development Tools

- `black>=24.0.0` - Code formatting
- `ruff>=0.1.0` - Linting
- `mypy>=1.8.0` - Type checking
- `pre-commit>=3.6.0` - Git hooks

## 📝 Example Test

```python
# tests/unit/test_resource_group_manager.py

import pytest
from unittest.mock import Mock, patch
from azure.core.exceptions import ResourceNotFoundError
from src.resource_group.manager import ResourceGroupManager


class TestResourceGroupManager:
    """Unit tests for ResourceGroupManager."""
    
    def test_create_resource_group_success(self, mock_credential):
        """Test successful resource group creation."""
        # ARRANGE
        manager = ResourceGroupManager(mock_credential)
        rg_name = "test-rg"
        location = "westeurope"
        
        with patch.object(manager, '_client') as mock_client:
            mock_client.resource_groups.create_or_update.return_value = Mock(
                name=rg_name,
                location=location
            )
            
            # ACT
            result = manager.create_resource_group(rg_name, location)
            
            # ASSERT
            assert result.name == rg_name
            assert result.location == location
            mock_client.resource_groups.create_or_update.assert_called_once()
    
    def test_create_resource_group_invalid_name(self, mock_credential):
        """Test resource group creation with invalid name."""
        # ARRANGE
        manager = ResourceGroupManager(mock_credential)
        invalid_name = ""
        
        # ACT & ASSERT
        with pytest.raises(ValueError, match="Resource group name cannot be empty"):
            manager.create_resource_group(invalid_name, "westeurope")
```

## 🔗 Related Repositories

- [learning-internal-development-platform](https://github.com/vanHeemstraSystems/learning-internal-development-platform) - Main overview repository
- [learning-idp-python-azure-sdk](https://github.com/vanHeemstraSystems/learning-idp-python-azure-sdk) - Azure SDK fundamentals
- [learning-idp-infrastructure-as-code](https://github.com/vanHeemstraSystems/learning-idp-infrastructure-as-code) - IaC patterns

## 🤝 Contributing

This is a personal learning repository, but suggestions and improvements are welcome!

1. Fork the repository
1. Create a feature branch
1. Make your changes with tests
1. Ensure all tests pass
1. Submit a pull request

## 📄 License

This project is for educational purposes. See LICENSE file for details.

## 📧 Contact

Willem van Heemstra

- GitHub: [@vanHeemstraSystems](https://github.com/vanHeemstraSystems)
- LinkedIn: [Willem van Heemstra](https://www.linkedin.com/in/willemvanheemstra/)

-----

*Last updated: December 18, 2025*
*Part of the learning-internal-development-platform series*

