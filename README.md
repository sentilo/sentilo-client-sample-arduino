# Sample for Sentilo client library for Arduino

These are some Sentilo client HTTP Request library sample sketches for Arduino and the Ethernet shield.

# Usage

### Include

You need to have the `Ethernet` library already included.

```c++
#include <Ethernet.h>
#include <SPI.h>
#include "SentiloClient.h"
```

### Run the sample code

* SentiloClient-Example-01.ino
  * basic example that connects to the Sentilo instance and publish one observation to an existing sensor
* SentiloClient-Example-02.ino
 * basic example that connects to the Sentilo instance and publish one observation to an existing sensor from two input devices: a LM35 temperature transistor and a LDR cedule
* SentiloClient-Example-03.ino
    * like the last two examples, this one creates the sensor if it doesn't exists in the catalog

### Configure the connection
You must provide some custom configuration before run these sample codes:

```c++
char* apiKey = "YOUR_API_KEY";
char* ip = "YOUR_IP_ADDRESS";
int port = YOUR_PORT;
```

Please, provide your credentials or api key, the Sentilo instance host ip and it port. After taht, you can upload the sketch to the Arduino devide.

We hope you enjoy it!
