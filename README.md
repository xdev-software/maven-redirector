# Maven Redirector

Publishes Maven redirect artifacts

## Usage

* Migrate the repository of the actual artifact from e.g. ``com.xdev-software:test`` to ``software.xdev:test``
* Release a new version of that artifact (e.g. 1.2.3 -> 2.0.0)
* Run the [deploy workflow](https://github.com/xdev-software/maven-redirector/actions/workflows/deploy.yml)https://github.com/xdev-software/maven-redirector/actions/workflows/deploy.yml of this repository with the following parameters:
  | Parameter | Example Value |
  | --- | --- |
  | Old GroupId | ``com.xdev-software`` |
  | New GroupId | ``software.xdev`` |
  | ArtifactId | ``test`` |
  | Version | ``2.0.0`` |
  | Url | ``https://github.com/xdev-software/test`` |
