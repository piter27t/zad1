# zad1_dodatkowe

## Punkt 2.
Zbudować  obrazy  kontenera  z  aplikacją  opracowaną  w  punkcie  nr  1,  które  będą  pracował  na 
architekturach: linux/arm/v7, linux/arm64/v8 oraz linux/amd64 wykorzystując sterownik docker-
container.

Stworzenie nowego builder-a:  ```docker buildx create --name labbuilder```

Ustawienie stworzonego builder-a: ```docker buildx use labbuilder```

Sprawdzenie stanu builder-a ```docker buildx inspect --bootstrap```

Zbudowanie obrazow dla dwoch architektur (linux/arm64/v8 oraz linux/amd64) Nie udalo sie stowrzyc obrazu dla linux/arm/v7: ```docker buildx build -t docker.io/piter27t/zad1_dod --platform linux/amd64,linux/arm64/v8 --push .```


