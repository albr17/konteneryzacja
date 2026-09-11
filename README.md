# Bioinformatyka Konteneryzacja 



# Opis projektu

Projekt wykorzystuje Docker Compose do uruchomienia środowiska bioinformatycznego składającego się z:

* usługi **FastQC** do analizy jakości danych sekwencjonowania,
* serwera **NGINX** udostępniającego wyniki przez przeglądarkę

## Wymagania
Przed uruchomieniem projektu należy zainstalować:
* Docker
* Docker Compose




## Budowanie i uruchamianie projektu
Uruchomienie wszystkiego:

```bash
docker compose up --build
```

Uruchomienie w tle:

```bash
docker compose up -d --build
```

## Sprawdzenie działania kontenerów

```bash
docker ps
```





## Dostęp do wyników
Po poprawnym uruchomieniu projektu wyniki są dostępne pod adresem:

```text
http://localhost:8080
```


## Używane obrazy

### FastQC
```text
biocontainers/fastqc:v0.11.9_cv8
```

### NGINX

```text
nginx:latest
```

