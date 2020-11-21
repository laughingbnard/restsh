## REST Shell (restsh)

Visual Studio Code Development Environment

This project is using [rust dev container](https://github.com/microsoft/vscode-dev-containers/tree/master/containers/rust) from Microsoft as boostrap base project. However, instead of using `.devcontainer\Dockerfile` directly, this project uses `.devcontainer\base.Dockerfile` to get independent of Microsoft's updating schedule for new rustc versions or to have the option to slim down the base image (see [rust image description at docker hub](https://hub.docker.com/_/rust) for more about alternative/slimer rust containers). The folder `.devcontainer\library-scripts` may have to be cloned manual from GitHub. 

Used crates:

- [rocket](https://crates.io/crates/rocket): Web framework
- [fern](https://crates.io/crates/fern): Logging
- [clap](https://crates.io/crates/clap): Command line argument parser and config files handling
- [indicatif](https://crates.io/crates/indicatif): progress bar
- [proptest](https://crates.io/crates/proptest): property testing

Considered crates:

- [dialoguer](https://crates.io/crates/dialoguer): command line prompts
- [console](https://crates.io/crates/console): terminal abstraction
- [chrono](https://crates.io/crates/chrono): Date/time
- [regex](https://crates.io/crates/regex): Regular expressions
- [heim](https://crates.io/crates/heim): system information
- [prettytable-rs](https://crates.io/crates/prettytable-rs): console printing of tabular data
- [mockito](https://crates.io/crates/mockito): http mocking
- [tracing](https://crates.io/crates/tracing): application level tracing
- [textwrap](https://crates.io/crates/textwrap): text wrapping
- [humantime](https://crates.io/crates/humantime): free-form time formatting and parsing
- [tempfile](https://crates.io/crates/tempfile): temporary files/directory management
