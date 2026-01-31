# Playwright Project

A comprehensive test automation suite built with Playwright for testing language conversion and UI functionality.

## Project Structure

```
.
├── pages/                      # Page Object Models
│   └── LanguageConversionPage.ts
├── tests/                      # Test files
│   ├── negative/              # Negative test scenarios
│   │   ├── neg-fun-0001-0005.spec.ts
│   │   └── neg-fun-0006-0010.spec.ts
│   ├── positive/              # Positive test scenarios
│   │   ├── pos-fun-0001-0010.spec.ts
│   │   ├── pos-fun-0011-0020.spec.ts
│   │   └── pos-fun-0021-0024.spec.ts
│   └── ui/                    # UI test scenarios
│       └── pos-ui-0001.spec.ts
├── scripts/                   # Utility scripts
│   ├── generateExcel.ts       # Generate Excel reports
│   ├── mock-server.ts         # Mock server setup
│   └── updateExcelResults.ts  # Update Excel with test results
├── utils/                     # Test utilities
│   ├── excelHelper.ts         # Excel handling utilities
│   └── testData.ts            # Test data
├── playwright.config.ts       # Playwright configuration
├── tsconfig.json              # TypeScript configuration
└── package.json               # Project dependencies
```

## Installation

1. Clone the repository:
```bash
git clone https://github.com/subasinghedewmini2-arch/full-Playwright-project.git
cd full-Playwright-project
```

2. Install dependencies:
```bash
npm install
```

## Running Tests

### Run all tests:
```bash
npx playwright test
```

### Run specific test suite:
```bash
# Positive tests
npx playwright test tests/positive

# Negative tests
npx playwright test tests/negative

# UI tests
npx playwright test tests/ui
```

### Run tests in headed mode:
```bash
npx playwright test --headed
```

### Run with debug mode:
```bash
npx playwright test --debug
```

## Mock Server

Start the mock server (if available):
```bash
npm run start:mock
```

## Viewing Test Reports

After running tests, view the HTML report:
```bash
npx playwright show-report
```

## Configuration

- **Playwright Config**: `playwright.config.ts` - Configure browsers, test settings, and reporting
- **TypeScript Config**: `tsconfig.json` - TypeScript compiler settings
- **Package.json**: Project dependencies and scripts

## Test Results

Test results are generated in:
- `test-results/` - Detailed test result data
- `playwright-report/` - HTML test report

## Technologies

- **Playwright** - Browser automation testing framework
- **TypeScript** - Type-safe test development
- **Node.js** - Runtime environment

## License

See LICENSE file for details.
