
# Flutter: Neumorphism Modern UI (Light Theme)

A flutter application to showcase how to create the Neumorphism effect.


## Deployment Setup

Clone the project

```bash
  git clone https://github.com/ckiggundu/neumorphism_flutter
```

Go to the project directory

```bash
  cd neumorphism_flutter
```

Install dependencies

```bash
  flutter pub get
```

Start the device emulator

```bash
  flutter run
```


## Usage/Examples

```dart
return Scaffold(
    // make the background color grey
      backgroundColor: Colors.grey[300],

      // place everything in a body and center it
      body: Center(
          
          // create the container that holds the shape
        child: Container(

            //insert the image into the shape
          child: Image.asset(
            'images/icons8-instagram-250.png',
            height: 80,
            color: Colors.grey[700],
          ),
          padding: const EdgeInsets.all(30),

          //create the shape
          decoration: BoxDecoration(
            color: Colors.grey[300],

            // rectangle with rounded edges
            //borderRadius: BorderRadius.circular(12),

            shape: BoxShape.circle,

            // make list of box shadows to use more than one
            boxShadow: [
                
              //bottom right shadow is darker
              BoxShadow(
                color: Colors.grey.shade500,
                offset: const Offset(4, 4),
                blurRadius: 15,
                spreadRadius: 1,
              ),

              //top left shadow is lighter
              const BoxShadow(
                color: Colors.white,
                offset: Offset(-4, -4),
                blurRadius: 15,
                spreadRadius: 1,
              ),
            ],
          ),
        ),
      ),
    );
```

## Screenshots

[![Screenshot-2022-06-16-153528.png](https://i.postimg.cc/Qt1J4dWW/Screenshot-2022-06-16-153528.png)](https://postimg.cc/KkcT4FfZ)

