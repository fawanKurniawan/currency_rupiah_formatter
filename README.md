# currency_rupiah_formatter

## Contoh Penggunaannya

```bash

import 'package:flutter/material.dart';

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
                FormatCurrency.convertToIdr(item.hargaProduk, 2),
                maxLines: 1,
                textAlign: TextAlign.left,
                style: TextStyle(
                  fontSize: 11,
                  color: Colors.orange,
          ),
        ),
      ),
    );
  }
}
```
