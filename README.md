 import 'package:flutter/material.dart';

void main() {
  runApp(benimuygulama());
}

class benimuygulama extends StatelessWidget {
  const benimuygulama({Key? key}) : super(key: key);

  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Scaffold(
        appBar: AppBar(
          backgroundColor: Colors.white,
          centerTitle: true,
          title: Text(
            "Bugün ne yesem",
            style: TextStyle(fontSize: 24, color: Colors.black),
          ),
        ),
        body: yemeksayfasi(),
      ),
    );
  }
}

class yemeksayfasi extends StatelessWidget {
  const yemeksayfasi({Key? key}) : super(key: key);

  @override
  Widget build(BuildContext context) {
    return Center(
      child: Column(
        children: <Widget>[
          Expanded(
            child: Padding(
              padding: const EdgeInsets.all(8.0),
              child: TextButton(
                  style: TextButton.styleFrom(primary: Colors.white),
                  onPressed: () {
                    print("Çorba");
                  },
                  child: Image.asset('assets/image/corba_$sayi.jpg')),
            ),
          ),
          Expanded(
            child: Padding(
              padding: const EdgeInsets.all(8.0),
              child: TextButton(
                  style: TextButton.styleFrom(primary: Colors.white),
                  onPressed: () {
                    print("Yemek");
                  },
                  child: Image.asset('assets/image/yemek_1.jpg')),
            ),
          ),
          Expanded(
            child: Padding(
              padding: const EdgeInsets.all(8.0),
              child: TextButton(
                  style: TextButton.styleFrom(primary: Colors.white),
                  onPressed: () {
                    print("Tatli");
                  },
                  child: Image.asset('assets/image/tatli_1.jpg')),
            ),
          ),
        ],
      ),
    );
  }
}
2. kodlar
