# currency_rupiah_formatter

## Contoh Penggunaannya

```bash


import 'package:flutter/material.dart';import 'package:intl/intl.dart';

void main() => runApp(MyApp());

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'Welcome to Flutter',
      home: Scaffold(
        appBar: AppBar(
          title: Text('Welcome to Flutter'),
        ),
        body: Center(
          child: Text(
                FormatCurrency.convertToIdr(10000, 2),
                maxLines: 1,
                textAlign: TextAlign.left,
                style: TextStyle(
                  fontSize: 11,
                  color: Colors.orange,)
          ),
        ),
      ),
    );
  }
}

      class FormatCurrency {
  static String convertToIdr(dynamic number, int decimalDigit) {
    NumberFormat currencyFormatter = NumberFormat.currency(
      locale: 'id',
      symbol: 'Rp ',
      decimalDigits: decimalDigit,
    );
    return currencyFormatter.format(number);
  }
}
```
