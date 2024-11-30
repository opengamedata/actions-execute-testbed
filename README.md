# actions-execute-testbed

Action to execute a testbed with Python's unittest test discovery

## Options

* `directory`: The directory in which test discovery should be performed, searching for the `test_file`
* `test_file`: The python file containing the testbed
* `python_version`: Which version of Python to install on local GitHub Actions runner (optional)

## Usage

```yaml
# For a module named `Module`
- name: Execute Module Testbed
    uses: opengamedata/actions-execute-testbed@v1.0
    with:
    directory: "tests/cases/utils"
    test_file: "t_Module.py"
    python_version: ${{ vars.OGD_PYTHON_VERSION }}
```
