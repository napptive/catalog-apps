# catalog-apps

A collection of OAM applications for the Napptive catalog

## Repository structure

The repository structure uses directories to organize applications by their associated version in the form of
`apps/<application_name>/<version>`.

Where:

* `application_name`: The name of the application as it will be shown in the catalog. This is typically associated with
the main component of the application.
* `version`: The version as it will be shown in the catalog. In a multi-component application use the version associated
with the image of the main component. Avoid when possible variable versions such as *latest*.

## Adding a new application

Contributions are welcomed to include new [applications](https://docs.napptive.com/app_management/what_is_an_app.html)
that will be made available on the Napptive Catalog to all [playground](https://napptive.com/platform/) users. To add a
new application, open a pull request following our [contribution guidelines](CONTRIBUTING.md). Before submitting the PR,
be sure that the application license enables the type of usage that you are intended to deploy. If you would like to see
a new application added, open an issue with the application details.

Once the PR gets accepted, we will periodically push the newer applications to the Playground platform.

## License

Copyright 2023 Napptive

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

      https://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
