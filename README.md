# ripgrep-prebuilt

[![Build Status](https://dev.azure.com/vscode/ripgrep-prebuilt/_apis/build/status/microsoft.ripgrep-prebuilt?branchName=main)](https://dev.azure.com/vscode/ripgrep-prebuilt/_build/latest?definitionId=18&branchName=main)

Builds [ripgrep](https://github.com/BurntSushi/ripgrep) on Azure Pipelines for multiple platforms, used by VS Code.

## Details

Reads `config.json` to determine which repo to clone and which tag to check out. If the build was triggered by a tag, each job will package the build outputs and publish them as pipeline artifacts, and the last job will upload those artifacts to the Github release. The Github release is consumed by the [vscode-ripgrep](https://github.com/microsoft/vscode-ripgrep) NPM package.

## Contributing

This project welcomes contributions and suggestions.  Most contributions require you to agree to a
Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
the rights to use your contribution. For details, visit https://cla.microsoft.com.

When you submit a pull request, a CLA-bot will automatically determine whether you need to provide
a CLA and decorate the PR appropriately (e.g., label, comment). Simply follow the instructions
provided by the bot. You will only need to do this once across all repos using our CLA.

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
