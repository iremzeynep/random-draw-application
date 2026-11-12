# Java Swing Random Draw Application (Çekiliş Uygulaması)

*Note: This project was developed as a practical application of concepts learned during a Udemy Java course to strengthen my skills in desktop UI development and File I/O.*

A desktop application built with Java Swing that allows users to randomly select winners from a text file. The application features a graphical user interface (GUI), dynamic file reading, and audio integration to play an applause sound effect when the winners are announced.

## Features

* **Graphical User Interface (GUI):** A clean and intuitive desktop interface built using Java Swing (JFrame).
* **Dynamic File I/O:** Users can browse and select a custom `.txt` file containing the list of participants.
* **Random Selection Algorithm:** The application safely reads the participant list, removes duplicates using a `Set` collection, and randomly selects up to 10 winners without freezing or entering infinite loops, even if the participant count is low.
* **Audio Integration:** Uses the `javax.sound.sampled` library to automatically play an applause sound effect (`.wav`) upon completing the draw.
* **State Reset:** Automatically clears previous participants and winners when a new draw is initiated.

## Tech Stack

* **Language:** Java (JDK 8+)
* **UI Framework:** Java Swing
* **Collections Used:** `ArrayList`, `TreeSet`, `DefaultListModel`
* **File Handling:** `JFileChooser`, `BufferedReader`, `FileInputStream`

## How to Run the Application

1. Clone this repository to your local machine.
2. Ensure you have the Java Development Kit (JDK) installed.
3. Open the project in an IDE that supports Java Swing (like NetBeans, IntelliJ IDEA, or Eclipse).
4. Run the `Cekilis.java` file.
5. In the application:
   * Click the **"Gözat"** (Browse) button to select the provided `katilanlar.txt` file (or any custom `.txt` file with names on separate lines).
   * Click the **"Çekiliş Yap"** (Draw) button to randomly select the winners.
   * Enjoy the applause!
