# Contributing Guidelines

Thank you for your interest in contributing to the **L-BFGS Solver Course** project.

We welcome improvements in:

- Mathematical derivations
- Algorithm correctness
- Numerical stability
- Code quality
- Benchmarking
- Documentation
- Tests
- Performance improvements

---

## Project Philosophy

This repository follows these principles:

- Mathematical correctness first
- Reproducible experiments
- Clean and readable implementation
- Minimal dependencies
- Transparent optimization logic

All contributions must respect these principles.

---

## How to Contribute

### 1. Fork the Repository

Fork the project and clone your fork locally:

```bash
git clone https://github.com/<your-username>/lbfgs-solver-course.git
cd lbfgs-solver-course

---

### 2. Create a Feature Branch

Always create a new branch for changes:

```bash
git checkout -b feature/your-feature-name
```

Branch naming examples:

* `feature/improve-two-loop`
* `feature/add-benchmark`
* `fix/line-search-bug`
* `docs/improve-theory`

---

### 3. Follow Code Standards

* Use clear variable names
* Add docstrings to functions
* Keep functions small and modular
* Avoid unnecessary abstraction

Python style:

```bash
black .
flake8 .
pytest
```

---

### 4. Add Tests (If Applicable)

If your contribution modifies solver logic:

* Add unit tests in `tests/`
* Test numerical stability
* Test convergence on quadratic functions

Pull requests without tests (for code changes) may require review discussion.

---

### 5. Update Documentation

If you modify:

* Algorithm behavior → Update theory docs
* API → Update README
* Implementation → Update documentation accordingly

Documentation must reflect code changes.

---

## Pull Request Process

1. Push your branch:

```bash
git push origin feature/your-feature-name
```

2. Open a Pull Request.

3. Include:

* Description of change
* Motivation
* Benchmark results (if performance changes)
* Test results

---

## Code Review Criteria

Your PR will be reviewed based on:

* Mathematical correctness
* Numerical stability
* Clean implementation
* Test coverage
* Documentation clarity

---

## Reporting Issues

If you find:

* Mathematical inconsistency
* Implementation bug
* Performance regression
* Documentation error

Open an Issue with:

* Clear description
* Minimal reproducible example
* Expected vs actual behavior

---

## Code of Conduct

Be respectful and constructive.

Focus on:

* Technical discussion
* Algorithm improvement
* Scientific correctness

---

Thank you for improving the project 

