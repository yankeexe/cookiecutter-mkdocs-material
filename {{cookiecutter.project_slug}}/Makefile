SHELL :=/bin/bash
CWD := $(PWD)
TMP_PATH := $(CWD)/.tmp
VENV_PATH := $(CWD)/venv

.PHONY: clean
.DEFAULT_GOAL := help

clean:
	@rm -rf $(TMP_PATH) __pycache__ .pytest_cache
	@find . -name '*.pyc' -delete
	@find . -name '__pycache__' -delete

venv: # Create a virtual environment
	@python3 -m venv venv

setup: # Install Developer Dependencies
	@pip install -r requirements.txt

run: # Server the docs on a local server
	mkdocs serve

help: # Show this help
	@egrep -h '\s#\s' $(MAKEFILE_LIST) | sort | awk 'BEGIN {FS = ":.*?# "}; {printf "\033[36m%-20s\033[0m %s\n", $$1, $$2}'