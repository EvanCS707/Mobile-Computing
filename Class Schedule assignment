import 'package:flutter/material.dart';

void main() {
  runApp(MyApp());
}

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'Class Schedule',
      theme: ThemeData(
        primarySwatch: Colors.blue,
      ),
      home: MyHomePage(),
    );
  }
}

class MyHomePage extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: Text('My Class Schedule'),
      ),
      body: Center(
        child: Column(
          mainAxisAlignment: MainAxisAlignment.center,
          children: <Widget>[
            Text(
              'Class Schedule:',
              style: TextStyle(fontSize: 20, fontWeight: FontWeight.bold),
            ),
            SizedBox(height: 20),
            ClassCard(day: 'Monday', subject: 'Scripting'),
            ClassCard(day: 'Wednesday', subject: 'Scripting'),
            ClassCard(day: 'Friday', subject: 'Scripting'),
            ClassCard(day: 'Tuesday', subject: 'Comp. Arch. & Mbile Comp.'),
            ClassCard(day: 'Thursday', subject: 'Comp. Arch. & Mbile Comp.'),
            SizedBox(height: 20),
            Icon(
              Icons.school,
              size: 50,
              color: Colors.blue,
            ),
          ],
        ),
      ),
    );
  }
}

class ClassCard extends StatelessWidget {
  final String day;
  final String subject;

  ClassCard({required this.day, required this.subject});

  @override
  Widget build(BuildContext context) {
    return Container(
      margin: EdgeInsets.symmetric(vertical: 5),
      padding: EdgeInsets.all(10),
      decoration: BoxDecoration(
        border: Border.all(color: Colors.blue),
        borderRadius: BorderRadius.circular(10),
      ),
      child: Row(
        mainAxisAlignment: MainAxisAlignment.spaceBetween,
        children: [
          Text(
            day,
            style: TextStyle(fontSize: 18),
          ),
          Text(
            subject,
            style: TextStyle(fontSize: 18),
          ),
        ],
      ),
    );
  }
}
