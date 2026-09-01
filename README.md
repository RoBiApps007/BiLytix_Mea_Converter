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
