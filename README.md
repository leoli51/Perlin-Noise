# Simplex-Noise based Map Generator
This is a java port of [Sebastian Lague](https://github.com/SebLague)'s map generetor, Thank you! <3. This version is based on the Simplex-Noise (the simplex noise implementation was written by [Stefan Gustavson](https://github.com/stegu)) algorithm. The map generator class uses the Vector2 LibGdx implementation but you can modify it to use any Pair/Point/Vector class.
## Usage example
```java
float[][] map = new float[height][width];
MapGenerator.GenerateNoiseMap(map, mapWidth, mapHeight, seed, scale, octaves, persistence, lacunarity, offset);

//Alternatively
float[][] map = MapGenerator.GenerateNoiseMap(mapWidth, mapHeight, seed, scale, octaves, persistence, lacunarity, offset);
```
