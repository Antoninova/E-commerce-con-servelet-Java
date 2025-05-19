# E-commerce-con-servelet-Java

## Cos’è il progetto
Un negozio online di scarpe realizzato con **Java Servlet** e **Gradle (Gradlew)**. Gli utenti possono navigare tra le card dinamiche dei prodotti, registrarsi, effettuare il login e gestire un carrello per completare l’acquisto. Dal lato amministratore, è possibile creare codici coupon e promozioni per festività o eventi speciali.

> ⚠️ **Nota:** non è possibile ospitare questo progetto su GitHub Pages, in quanto utilizza un _build system_ Gradle e richiede un _servlet container_ (es. Tomcat).

---

## Perché questo progetto
Ho scelto di sviluppare un e-commerce in Java Servlet per mettere in pratica:
- Il ciclo di vita delle servlet  
- La gestione di sessioni e cookie  
- L’integrazione con database (JDBC)  
- L’architettura MVC minimale  

Inoltre, ho voluto replicare le funzionalità reali di un negozio online, inclusi sconti e gestione amministrativa.

---

## Il mio “Capolavoro”
L’applicazione comprende:

1. **Home & Catalogo**  
   - Card dinamiche generate a partire dai dati del database  
   - Filtri per modello, taglia e colore  

2. **Carrello**  
   - Aggiunta/rimozione prodotti in sessione  
   - Calcolo di subtotale, imposte e totale  

3. **Autenticazione**  
   - **Registrazione**: form con validazione lato server  
   - **Login/Logout**: gestione sicura di password hashed  

4. **Area Amministratore**  
   - Creazione e validazione di **codici coupon** (sconti percentuali o fissi)  
   - Programmazione di promozioni festive (es. Natale, Saldi estivi)  
   - CRUD su catalogo prodotti  

5. **Checkout**  
   - Riepilogo ordine con possibilità di applicare coupon  
   - Conferma d’acquisto e notifica via email (JavaMail)  

---

## Link al progetto

- [Codice sorgente su GitHub](https://github.com/Antoninova/ECommerce-Servlets)  
- ⚙️ **Deploy locale:**  
  1. Clona la repo  
  2. `./gradlew build`  
  3. Copia il WAR in `webapps/` di Tomcat  
  4. Avvia Tomcat e visita `http://localhost:8080/ecommerce`  
