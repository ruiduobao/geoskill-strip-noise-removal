---
name: geoskill-strip-noise-removal
description: '去除 Landsat7 SLC-off / MODIS 等条带噪声，支持矩匹配与加权线性回归。Destriping for Landsat7 SLC-off / MODIS via moment matching and weighted linear regression; outputs a corrected GeoTIFF and gap mask.'
---

# 条带噪声去除 | Strip Noise Removal

(Fill in 2-3 paragraphs of introduction here: features, application scenarios, core algorithm.)

## Dependencies / 依赖

```bash
pip install 'numpy' 'rasterio' 'scipy'
```

## Usage / 使用方法

### Basic Usage

```bash
python geoskill-strip-noise-removal.py --bbox 116.0 39.0 117.0 40.0 [other arguments]
```

### Example 1 (synthetic data, offline)

```bash
python geoskill-strip-noise-removal.py --bbox 116.0 39.0 117.0 40.0 --synthetic --output-dir ./out
```

### Examples 2-5

(Add at least 4 real usage examples.)

## Output / 输出

| File | Format | Description |
|---|---|---|
| `result.tif` | GeoTIFF | Primary output |
| `output-manifest.json` | JSON | Run manifest |

## Data Source / 数据源 / Source

(Describe the data source: free satellite data / local input / synthetic.)

## Privacy / 隐私声明 / Privacy

- Runs offline by default; `--synthetic` mode requires no network at all.
- All processing is done locally; user data is never uploaded.

## License / License

MIT

---

> 中文完整版：需要时再读 [references/SKILL.zh-CN.md](references/SKILL.zh-CN.md)，不要默认全量加载。
