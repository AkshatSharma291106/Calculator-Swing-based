# Calculator & Pomodoro Timer Applications

A Java-based calculator application with multiple themes and a separate Pomodoro timer utility.

## 📁 Project Structure

This repository contains two main applications:

### 1. Calculator Application


A feature-rich calculator with both standard and scientific modes, supporting multiple visual themes.

#### Features:
- **Dual Modes**: Standard calculator and Scientific calculator with advanced functions
- **Theme Support**: Light and Dark themes with customizable colors
- **Mathematical Operations**:
  - Basic: +, -, ×, ÷, %
  - Scientific: Square root (√), Power (pow), Natural logarithm (ln)
- **User-Friendly Interface**: Clean GUI with intuitive button layout

#### Key Components:
- `App.java` - Main application entry point
- `CalculatorUI.java` - Main user interface class
- Theme management system with YAML configuration
- Comprehensive unit tests

### 2. Pomodoro Timer Application
**Location**: `org.example`

A simple countdown timer application designed for Pomodoro technique productivity.

#### Features:
- **25-minute countdown timer** (standard Pomodoro duration)
- **Minimalist interface** that stays on top of other windows
- **Real-time display** of remaining time

#### Key Components:
- `Main.java` - Application entry point
- `GUI.java` - User interface implementation
- `CountdownTimer.java` - Timer logic and countdown management

## 🛠️ Technologies Used

- **Java Swing** - For GUI components
- **Maven** - Dependency management and build automation
- **JUnit 5** - Unit testing framework
- **Jackson YAML** - For theme configuration parsing
- **Java Timer API** - For countdown functionality

## 📦 Build & Run

### Prerequisites
- Java JDK 24+
- Maven 3.6+

### Building the Project
```bash
mvn clean compile
```

### Running the Calculator
```bash
mvn exec:java -Dexec.mainClass="com.houarizegai.calculator.App"
```

### Running the Pomodoro Timer
```bash
mvn exec:java -Dexec.mainClass="org.example.Main"
```

### Running Tests
```bash
mvn test
```

## 🎨 Theme Configuration

The calculator supports customizable themes defined in `src/main/resources/application.yaml`:

```yaml
themes:
  - name: Light
    applicationBackground: f0f3f9
    textColor: 000000
    operatorBackground: f7f9fc
    numbersBackground: ffffff
    btnEqualTextColor: ffffff
    btnEqualBackground: 0067c0
  - name: Dark
    applicationBackground: 1c2028
    textColor: ffffff
    operatorBackground: 2d333d
    numbersBackground: 363c47
    btnEqualTextColor: ffffff
    btnEqualBackground: 4cc2ff
```

## 📊 Calculator Operations

| Operation | Symbol | Example |
|-----------|--------|---------|
| Addition | + | 5 + 3 = 8 |
| Subtraction | - | 10 - 4 = 6 |
| Multiplication | * | 6 × 7 = 42 |
| Division | / | 15 ÷ 3 = 5 |
| Modulo | % | 10 % 3 = 1 |
| Square Root | √ | √9 = 3 |
| Power | pow | 2^3 = 8 |
| Natural Log | ln | ln(e) = 1 |

## 🔧 Development

### IDE Configuration
- The project includes IntelliJ IDEA configuration files
- Uses Java SDK 24
- Maven-based project structure

### Code Style
- Follows Java naming conventions
- Comprehensive JavaDoc documentation
- Unit tests for calculator logic

## 📝 License

This project is for educational purposes. Feel free to use and modify as needed.

## 👨‍💻 Author

Developed as a learning project for Java Swing applications and GUI development.

