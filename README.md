# Encoder-Brick
 
 This is a small board that implements a typical quadrature encoder. It includes provisions for hardware debouncing the A/B
 pins on the encoder. It also can optionally support a click button built into the encoder unit, too.
 
 
 ## Debouncing circuit
 
 Two of these circuits are on the board. Note that the "internal" resistor indicated is the internal pin PULLUP resistor
 on an Arduino-ish board. If your intended use case doesn't have internal pullups, you might need to add resistors to make
 this circuit work.

```
      (internal 20k)       10k
 pin:<---/\/\--------*----/\/\----|
                     |            |
              0.1uf ===            / switch
                     |            /
 gnd:<---------------*------------|
 ```
 
 ## Bill of Materials
 
 - [encoder](https://www.mouser.com/ProductDetail/Bourns/PEC11R-4215F-S0024?qs=Zq5ylnUbLm5lAqmKF80wzQ%3D%3D)
 - [a 4 pin header/connector with .1" pitch](https://www.mouser.com/ProductDetail/molex/22-23-2042/?qs=52ipEG6BoUGnVIQV2y3Jgg%3D%3D&countrycode=US&currencycode=USD)
 - 2x 10k axial lead resistors (whatever you have on hand should work)
 - 2x [0.1uF ceramic capacitor](https://www.mouser.com/ProductDetail/Vishay-BC-Components/K104K15X7RF53H5?qs=sGAEpiMZZMuMW9TJLBQkXpsARSeHIOPdD%2FiGrRofazY%3D) (again, whatever you have with the right value should work)
 
 Any quadrature encoder with the same footprint will work - there are a bunch, with various shaft lengths and styles!
 You may also want a knob. 
 
 
