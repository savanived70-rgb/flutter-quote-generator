import 'dart:math';
import 'package:flutter/material.dart';

void main() {
  runApp(const MyApp());
}

class MyApp extends StatelessWidget {
  const MyApp({super.key});

  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      debugShowCheckedModeBanner: false,
      home: QuoteApp(),
    );
  }
}

class QuoteApp extends StatefulWidget {
  @override
  State<QuoteApp> createState() => _QuoteAppState();
}

class _QuoteAppState extends State<QuoteApp> {
  final List<String> quotes = [
    "Believe in yourself.",
    "Dream big.",
    "Stay positive.",
    "Never give up.",
    "Success starts with you.",
    "Work hard, stay humble.",
    "Make today amazing.",
    "You are stronger than you think.",
    "Push yourself.",
    "Focus on progress.",
    "Small steps matter.",
    "Be fearless.",
    "Create your future.",
    "Stay motivated.",
    "Think positive.",
    "Learn every day.",
    "Trust the process.",
    "Do your best.",
    "Be kind.",
    "Stay focused.",
    "Never stop learning.",
    "Chase your dreams.",
    "You can do it.",
    "Stay strong.",
    "Rise and shine.",
    "Keep moving forward.",
    "Be confident.",
    "Stay inspired.",
    "Believe & achieve.",
    "Turn dreams into plans.",
    "Keep going.",
    "Smile more.",
    "Hard work pays off.",
    "Stay curious.",
    "Be proud of yourself.",
    "Enjoy the journey.",
    "Stay brave.",
    "No pain, no gain.",
    "Make it happen.",
    "Stay happy.",
    "Think big.",
    "Be unstoppable.",
    "Stay calm.",
    "Grow every day.",
    "Win your mind.",
    "Never quit.",
    "Positive vibes.",
    "Believe in magic.",
    "Success is coming.",
    "You matter."
  ];

  String currentQuote = "Tap the button for a quote!";

  void generateQuote() {
    final random = Random();
    setState(() {
      currentQuote = quotes[random.nextInt(quotes.length)];
    });
  }

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      body: Container(
        decoration: const BoxDecoration(
          gradient: LinearGradient(
            colors: [Colors.deepPurple, Colors.blue],
            begin: Alignment.topLeft,
            end: Alignment.bottomRight,
          ),
        ),
        child: Center(
          child: Padding(
            padding: const EdgeInsets.all(20),
            child: Column(
              mainAxisAlignment: MainAxisAlignment.center,
              children: [
                Card(
                  shape: RoundedRectangleBorder(
                    borderRadius: BorderRadius.circular(20),
                  ),
                  elevation: 10,
                  child: Padding(
                    padding: const EdgeInsets.all(25),
                    child: Text(
                      currentQuote,
                      textAlign: TextAlign.center,
                      style: const TextStyle(
                        fontSize: 24,
                        fontWeight: FontWeight.bold,
                      ),
                    ),
                  ),
                ),

                const SizedBox(height: 40),

                ElevatedButton(
                  style: ElevatedButton.styleFrom(
                    padding: const EdgeInsets.symmetric(
                        horizontal: 30, vertical: 15),
                    shape: RoundedRectangleBorder(
                      borderRadius: BorderRadius.circular(30),
                    ),
                  ),
                  onPressed: generateQuote,
                  child: const Text(
                    "Generate Quote",
                    style: TextStyle(fontSize: 18),
                  ),
                ),
              ],
            ),
          ),
        ),
      ),
    );
  }
}
