# Maven Redirector

Publishes Maven redirect artifacts

## Usage

* Migrate the repository of the actual artifact from e.g. ``software.xdev:test`` to ``software.xdev:test2``
* Release a new version of that artifact (e.g. 1.2.3 -> 2.0.0)
* Run the [deploy workflow](https://github.com/xdev-software/maven-redirector/actions/workflows/deploy.yml) of this repository with the following parameters:
  | Parameter | Example Value |
  | --- | --- |
  | Old GroupId | ``software.xdev`` |
  | New GroupId | ``software.xdev`` |
  | Old ArtifactId | ``test`` |
  | New ArtifactId | ``test-2`` |
  | Version | ``2.0.0`` |
