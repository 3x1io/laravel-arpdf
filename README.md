#### Laravel ArPDF
# Laravel ArPDF

A Laravel package for generating PDF files with support for both English and Arabic languages without relying on external libraries.

## Installation

To install the `laravel-arpdf` package, follow these steps:

1. **Add the package to your Laravel project using Composer**:

   ```bash
   composer require baidouabdellah/laravel-arpdf
   ```

2. **Register the Service Provider (if using Laravel < 5.5)**:

   In your `config/app.php` file, add the following line to the `providers` array:

   ```php
   Baidouabdellah\LaravelArpdf\ArPDFServiceProvider::class,
   ```

3. **Publish the configuration file (optional)**:

   You can publish the configuration file to customize the package settings:

   ```bash
   php artisan vendor:publish --provider="Baidouabdellah\LaravelArpdf\ArPDFServiceProvider"
   ```

## Usage

To use the package, you can access the PDF generation functionality using the following command:

```php
$pdf = app('ArPDF');
// Add your PDF generation logic here
```

### Generating a PDF

Here’s an example of how to generate a simple PDF:

```php
$pdf = app('ArPDF');
$pdf->setTitle('Sample PDF');
$pdf->addPage();
$pdf->writeHTML('<h1>Hello World</h1>');
$pdf->output('sample.pdf');
```

## Support

If you encounter any issues, please open an issue on the [GitHub repository](https://github.com/baidou5/laravel-arpdf/issues).
 
# pleas Contact me 
Abdellah Baidou
Phone: +212 661-176711
Email: baidou.abd@gmail.com

## License

This package is licensed under the MIT License. See the [LICENSE](LICENSE) file for more information.
```
