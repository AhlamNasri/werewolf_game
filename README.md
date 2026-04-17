# Loup-Garou (Spring Boot + Thymeleaf)

## Démarrer

Prérequis:
- Java 17+ (Java 21 OK)
- Maven (ou IntelliJ)

### Avec Maven
```bash
mvn spring-boot:run
```

### Puis ouvre
- App: http://localhost:8080/
- H2 Console: http://localhost:8080/h2
  - JDBC URL: jdbc:h2:file:./data/werewolf
  - user: sa
  - password: (vide)

## Flux du jeu
1. Inscription / Connexion
2. Jouer → créer une room (admin) ou rejoindre avec la clé
3. Admin lance la partie (minimum 5 joueurs)
4. Nuit: Loups → Voyante → Sorcière
5. Jour: Discussion (chat) → Vote
6. Victoire: Village (plus de loups) ou Loups (loups >= autres)
