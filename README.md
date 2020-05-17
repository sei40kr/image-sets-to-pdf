# image-sets-to-pdf

Convert image sets to PDF so that I can read them on Google Play Books.

## Requirements

- ImageMagick
- UnRAR

## Usage

``` sh
image-sets-to-pdf [DIRECTORY OR ARCHIVE ...]
```

## Configurations

| Variable                  | Default value                     | Description                                                                                                                                                             |
|:--------------------------|:----------------------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `IMAGE_SET_SIZE_THRESOLD` | `3`                               | If the number of images in a directory is equal or larger than this value, this program converts them into a PDF.                                                       |
| `IMAGE_QUALITY`           | `90%`                             | The quality of images. This value will be passed to ImageMagick. This is useful to reduce the size of output file to avoid the upload limitations on Google Play Books. |
| `IMAGE_WIDTH`             | `''`                              | The width of output images.  images.                                                                                                                                           |
| `IMAGE_HEIGHT`            | `1024`                            | The height of output images.  images.                                                                                                                                          |
| `PDF_FILENAME_TEMPLATE`   | `'{series_name} {series_no}.pdf'` | The template for output PDF filenames. You can use these placeholders: `{series_name}` -> series name, `{series_no}` -> series no                                       |
