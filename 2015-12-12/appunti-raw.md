
Laravel

Risorse 


### Composer
Composer è un packet manager

composer global require "laravel/laravel"

laravel new task


convention over configuration

Se tu segui una determinata convenzione, tutto funziona più semplicemente e molto più velocemente. Ogni cosa al suo posto, e modulare.

### Vantaggi del file .env
Il file .env permette di avere configurazioni differenti a seconda del server in cui gira l'applicazione


## Panoramica sulla struttura base di una nuova applicazione laravel


### Driver



Come funzionano le request

Driver
Router
Controller -> comandare il flusso della richiesta. Il controller dovrebbe essere "magro". Non deve fare richieste al database. Non deve elaborare dati. Prende i dati dalla richiesta, li richiede alla model, li passa alla view.

Thin Controller / Thin Model / Big Repository


Middleware
Si occupano di gestire la richiesta che arriva, o di modificare la risposta. Ad esempio se un utente richiede una lista di dati (es.: my.app/users/list), un Middleware può verificare se l'utente è autorizzato ad esereguire quel comando. In caso contrario, l'utente viene ridirezionato ad una finestra di login (ridireziona a my.app/login)

Il vantaggio di un Middleware può essere quello ad esempio di riformattare dato di tipo "date" passata da un form, per riformattarlo in formato timestamp.

Esempio [ChekcForMaintenanceMode](http://laravel.com/docs/5.1#maintenance-mode)

Providers

Config

SomeRandomKey

Eloquent ORM




Le migrazioni di Laravel

Model




Dependency Injection
Sul sito laravel sono spiegate le [dependency injection](http://laravel.com/docs/5.1/container)

Service Container 
Sono uno strumento che ci permette

Si consiglia di consultare la documentazione di laravel, realizzata molto bene




