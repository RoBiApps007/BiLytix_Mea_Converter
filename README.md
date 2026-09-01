# BiLytix_Mea_Converter

Swift + Python scaffold for converting CSV measurement files to MF4.

## Current scaffold

- Swift package target: `BiLytix_Mea_Converter`
- Python conversion entrypoint: `Scripts/convert_csv_to_mf4.py`
- Input data folder: `data/input`
- Output data folder: `data/output`

## Local checks

```bash
swift test
python3 Scripts/convert_csv_to_mf4.py data/input/example.csv data/output/example.mf4
```

## GitHub Actions: build unsigned IPA

This repository includes a workflow at
`/home/runner/work/BiLytix_Mea_Converter/BiLytix_Mea_Converter/.github/workflows/build-unsigned-ipa.yml`
that builds an unsigned `.ipa` on macOS.

Set these repository variables when your iOS app project is available:

- `IOS_SCHEME` (recommended): Xcode scheme to build
- `IOS_WORKSPACE` (optional): workspace path, e.g. `App/App.xcworkspace`
- `IOS_PROJECT` (optional): project path, e.g. `App/App.xcodeproj`

If workspace/project variables are not set, the workflow auto-detects when there is exactly one
`.xcworkspace` or one `.xcodeproj` in the repository.
