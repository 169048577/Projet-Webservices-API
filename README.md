Description
Ce projet implémente des services web RESTful et SOAP pour la gestion des comptes bancaires, permettant aux clients et partenaires d'interagir avec leurs comptes. Les fonctionnalités principales incluent :

Consultation du solde du compte ( GET /accounts/{accountId}/balancepour REST et getBalance(accountId)pour SOAP)
Historique des transactions ( GET /accounts/{accountId}/transactionspour REST et getTransactions(accountId, pageNumber, pageSize)pour SOAP)
Effectuer un virement ( POST /accounts/{accountId}/transferpour REST et transferFunds(creditor, debtor, amount, currency)pour SOAP)
L'API REST est documentée avec Swagger et OpenAPI, et le service SOAP est décrit via un fichier WSDL.

Environnement
Pour développer et exécuter ce projet, vous aurez besoin des éléments suivants :

Outils de développement
IDE : Apache NetBeans 12.0 ou supérieur
Serveur d'Applications : Apache Tomcat 9.x ou supérieur
Kit de développement Java (JDK) : Java SE 8 ou supérieur
Profilage et Tests de Charge :
NetBeans Profiler pour analyser l'utilisation des ressources
Apache JMeter ou Gatling pour effectuer des tests de charge
Environnement de Développement
Système d'exploitation : Windows, macOS, ou Linux
Base de données : MySQL 5.7 ou supérieur (en option, si une base de données est utilisée pour stocker les comptes et transactions)
Dépendances
Pour ce projet, les dépendances suivantes sont nécessaires. Ces dépendances sont gérées via Maven et sont spécifiées dans le fichier pom.xmldu projet.

API REST
Spring Boot (pour la gestion des services RESTful)
Spring Data JPA (pour l'accès aux données via les référentiels)
Swagger (pour la documentation de l'API)
API SAVON
Spring-WS (pour la création des services SOAP)
JAXB (pour la liaison XML-Java dans les services SOAP)
Autres dépendances
Log4j (pour la gestion des logs)
JUnit (pour les tests unitaires)
Apache Commons (utilitaires supplémentaires)
Les fichiers JAR nécessaires doivent être placés dans le dossier libdu projet, ou ajoutés via Maven dans le fichier pom.xml.
