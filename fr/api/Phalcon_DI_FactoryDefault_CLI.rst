Class **Phalcon\\Di\\FactoryDefault\\Cli**
==========================================

*extends* class :doc:`Phalcon\\Di\\FactoryDefault <Phalcon_Di_FactoryDefault>`

*implements* :doc:`Phalcon\\DiInterface <Phalcon_DiInterface>`, ArrayAccess

Phalcon\\Di\\FactoryDefault\\CLI  This is a variant of the standard Phalcon\\Di. By default it automatically registers all the services provided by the framework. Thanks to this, the developer does not need to register each service individually. This class is specially suitable for CLI applications


Methods
-------

public  **__construct** ()

Phalcon\\Di\\FactoryDefault\\CLI constructor



public  **setInternalEventsManager** (*unknown* $eventsManager) inherited from Phalcon\\Di

Sets the internal event manager



public  **getInternalEventsManager** () inherited from Phalcon\\Di

Returns the internal event manager



public  **set** (*unknown* $name, *unknown* $definition, [*unknown* $shared]) inherited from Phalcon\\Di

Registers a service in the services container



public  **setShared** (*unknown* $name, *unknown* $definition) inherited from Phalcon\\Di

Registers an "always shared" service in the services container



public  **remove** (*unknown* $name) inherited from Phalcon\\Di

Removes a service in the services container



public  **attempt** (*unknown* $name, *unknown* $definition, [*unknown* $shared]) inherited from Phalcon\\Di

Attempts to register a service in the services container Only is successful if a service hasn"t been registered previously with the same name



public  **setRaw** (*unknown* $name, *unknown* $rawDefinition) inherited from Phalcon\\Di

Sets a service using a raw Phalcon\\Di\\Service definition



public  **getRaw** (*unknown* $name) inherited from Phalcon\\Di

Returns a service definition without resolving



public  **getService** (*unknown* $name) inherited from Phalcon\\Di

Returns a Phalcon\\Di\\Service instance



public  **get** (*unknown* $name, [*unknown* $parameters]) inherited from Phalcon\\Di

Resolves the service based on its configuration



public *mixed*  **getShared** (*string* $name, [*array* $parameters]) inherited from Phalcon\\Di

Resolves a service, the resolved service is stored in the DI, subsequent requests for this service will return the same instance



public  **has** (*unknown* $name) inherited from Phalcon\\Di

Check whether the DI contains a service by a name



public  **wasFreshInstance** () inherited from Phalcon\\Di

Check whether the last service obtained via getShared produced a fresh instance or an existing one



public  **getServices** () inherited from Phalcon\\Di

Return the services registered in the DI



public  **offsetExists** (*unknown* $name) inherited from Phalcon\\Di

Check if a service is registered using the array syntax



public *boolean*  **offsetSet** (*string* $name, *mixed* $definition) inherited from Phalcon\\Di

Allows to register a shared service using the array syntax 

.. code-block:: php

    <?php

    $di["request"] = new \Phalcon\Http\Request();




public *mixed*  **offsetGet** (*string* $name) inherited from Phalcon\\Di

Allows to obtain a shared service using the array syntax 

.. code-block:: php

    <?php

    var_dump($di["request"]);




public  **offsetUnset** (*unknown* $name) inherited from Phalcon\\Di

Removes a service from the services container using the array syntax



public *mixed*  **__call** (*string* $method, [*array* $arguments]) inherited from Phalcon\\Di

Magic method to get or set services using setters/getters



public static  **setDefault** (*unknown* $dependencyInjector) inherited from Phalcon\\Di

Set a default dependency injection container to be obtained into static methods



public static  **getDefault** () inherited from Phalcon\\Di

Return the lastest DI created



public static  **reset** () inherited from Phalcon\\Di

Resets the internal default DI



