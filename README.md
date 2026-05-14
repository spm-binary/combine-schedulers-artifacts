# combine-schedulers-artifacts

Build-and-release automation for `combine-schedulers` XCFramework artifacts.

Upstream package:
`https://github.com/pointfreeco/combine-schedulers`

Artifacts produced by this repository are consumed by:
`https://github.com/spm-binary/combine-schedulers.git`

## Release Flow

Run the `Build release` workflow with:

- `upstream_ref`: upstream tag or branch to build, such as `1.1.0`
- `release_tag`: release tag to create in this repository, usually the same
  semantic version

The workflow builds `CombineSchedulers` as an XCFramework zip asset and uploads
a `checksums.txt` file containing the SwiftPM checksum.
