# netCDF 轉換工具

這個專案包含兩個 Python 模組，用於操作 netCDF 格式的檔案。第一個模組 `netcdf_to_csv.py` 可將 netCDF 檔案轉換成 CSV 格式。第二個模組 `netcdf_meta.py` 可用來檢視 netCDF 檔案的元數據信息。

## 安裝

首先，使用以下命令安裝所需的套件：

```bash
python3 -m pip install netcdf-to-csv netcdf-meta
```

## 模組使用

### netcdf_to_csv

這個模組將 netCDF 檔案轉換成 CSV 格式。以下為使用方法和範例：

```bash
python3 -m netcdf_to_csv <nc_file1> <nc_file2> ...
```

範例：

```bash
python3 -m netcdf_to_csv example1.nc example2.nc
```

這將會將 `example1.nc` 和 `example2.nc` 轉換成對應的 CSV 檔案 `example1.csv` 和 `example2.csv`。

### netcdf_meta

這個模組用來檢視 netCDF 檔案的元數據信息。以下為使用方法和範例：

```bash
python3 -m netcdf_meta <nc_file1> <nc_file2> ...
```

範例：

```bash
python3 -m netcdf_meta example1.nc example2.nc
```

這將會顯示 `example1.nc` 和 `example2.nc` 的元數據信息，包括全局屬性、維度、變量和前三行數據。