## Description
**PLib** est une bibliothèque C++ dont l'objectif est de mettre en code tous les concepts vue en Prépa 

## Polynômes
Les polynômes sont décrits comme suit :
```cpp
class Polynomial 
{

public:
  Polynomial();
  Polynomial(std::vector<float> coef);
  int degree = 0;
  
  Polynomial operator+(Polynomial const& obj);
  Polynomial operator-(Polynomial const& obj);
  Polynomial operator*(Polynomial const& obj);
  Polynomial operator+(float const& obj);
  Polynomial operator*(float const& obj);
  Polynomial operator-(float const& obj);
  float operator()(float x);

  std::string ToString();

private:
  std::vector<float> coefficients;
};
```
On peut ainsi les utiliser de la manière suivante : 
```cpp
Polynomial P({0, 1, -3.5}); // P(x) = x - 3.5x²
float r = P(2); // r = 2 - 14 = -12
```