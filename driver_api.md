h1. Wing API Wing API documentation

*Version:* 0.0.1

----

{toc:printable=true|style=square|minLevel=2|maxLevel=3|type=list|outline=false|include=.*}

h2. Endpoints

    h3. driverAuthorizeUsingPOST
    {status:colour=Yellow|title=post|subtle=false}
    {code}
    post /api/v1/driver/authenticate
    {code}
    *Summary:* driverAuthorize
    *Description:*


    h4. Parameters

        h5. Body Parameter
        ||Name||Description||Required||Default||Pattern||
        |loginDTO |loginDTO |(/) | |  |







    h4. Responses
        *Status Code:* 200
        *Message:*     OK
        {code:title=Response Type}
JSendOfUserJWTToken
        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "OK",
  "schema" : {
    "$ref" : "#/definitions/JSendOfUserJWTToken"
  }
}
        {code}
        *Status Code:* 201
        *Message:*     Created
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Created"
}
        {code}
        *Status Code:* 401
        *Message:*     Unauthorized
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Unauthorized"
}
        {code}
        *Status Code:* 403
        *Message:*     Forbidden
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Forbidden"
}
        {code}
        *Status Code:* 404
        *Message:*     Not Found
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Not Found"
}
        {code}
    ----

    h3. getCallTimingForDriverUsingGET
    {status:colour=Yellow|title=get|subtle=false}
    {code}
    get /api/v1/driver/call-timings
    {code}
    *Summary:* getCallTimingForDriver
    *Description:*


    h4. Parameters



        h5. Query Parameters
        ||Name||Description||Required||Default||Pattern||
        |orderId |Order Id |(x) | |  |





    h4. Responses
        *Status Code:* 200
        *Message:*     OK
        {code:title=Response Type}
JSendOfListOfCallTimingsDTO
        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "OK",
  "schema" : {
    "$ref" : "#/definitions/JSendOfListOfCallTimingsDTO"
  }
}
        {code}
        *Status Code:* 401
        *Message:*     Unauthorized
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Unauthorized"
}
        {code}
        *Status Code:* 403
        *Message:*     Forbidden
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Forbidden"
}
        {code}
        *Status Code:* 404
        *Message:*     Not Found
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Not Found"
}
        {code}
    ----

    h3. butchUpdateOrdersDriverUsingPOST
    {status:colour=Yellow|title=post|subtle=false}
    {code}
    post /api/v1/driver/warehouse
    {code}
    *Summary:* butchUpdateOrdersDriver
    *Description:*


    h4. Parameters

        h5. Body Parameter
        ||Name||Description||Required||Default||Pattern||
        |dto |dto |(/) | |  |







    h4. Responses
        *Status Code:* 200
        *Message:*     OK
        {code:title=Response Type}
JSend
        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "OK",
  "schema" : {
    "$ref" : "#/definitions/JSend"
  }
}
        {code}
        *Status Code:* 201
        *Message:*     Created
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Created"
}
        {code}
        *Status Code:* 401
        *Message:*     Unauthorized
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Unauthorized"
}
        {code}
        *Status Code:* 403
        *Message:*     Forbidden
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Forbidden"
}
        {code}
        *Status Code:* 404
        *Message:*     Not Found
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Not Found"
}
        {code}
    ----

    h3. checkInToWarehouseUsingPOST
    {status:colour=Yellow|title=post|subtle=false}
    {code}
    post /api/v1/driver/check_in/warehouse/{warehouseId}
    {code}
    *Summary:* checkInToWarehouse
    *Description:*


    h4. Parameters
        h5. Path Parameters
        ||Name||Description||Required||Default||Pattern||
        |warehouseId |warehouseId |(/) | |  |








    h4. Responses
        *Status Code:* 200
        *Message:*     OK
        {code:title=Response Type}
JSendOfSelectItem
        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "OK",
  "schema" : {
    "$ref" : "#/definitions/JSendOfSelectItem"
  }
}
        {code}
        *Status Code:* 201
        *Message:*     Created
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Created"
}
        {code}
        *Status Code:* 401
        *Message:*     Unauthorized
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Unauthorized"
}
        {code}
        *Status Code:* 403
        *Message:*     Forbidden
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Forbidden"
}
        {code}
        *Status Code:* 404
        *Message:*     Not Found
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Not Found"
}
        {code}
    ----

    h3. createCustomerProfileUsingPOST
    {status:colour=Yellow|title=post|subtle=false}
    {code}
    post /api/v1/driver/create
    {code}
    *Summary:* createCustomerProfile
    *Description:*


    h4. Parameters

        h5. Body Parameter
        ||Name||Description||Required||Default||Pattern||
        |driverDto |driverDto |(/) | |  |







    h4. Responses
        *Status Code:* 200
        *Message:*     OK
        {code:title=Response Type}
JSendOfDriverDTO
        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "OK",
  "schema" : {
    "$ref" : "#/definitions/JSendOfDriverDTO"
  }
}
        {code}
        *Status Code:* 201
        *Message:*     Created
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Created"
}
        {code}
        *Status Code:* 401
        *Message:*     Unauthorized
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Unauthorized"
}
        {code}
        *Status Code:* 403
        *Message:*     Forbidden
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Forbidden"
}
        {code}
        *Status Code:* 404
        *Message:*     Not Found
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Not Found"
}
        {code}
    ----

    h3. getDriverAccountUsingGET
    {status:colour=Yellow|title=get|subtle=false}
    {code}
    get /api/v1/driver/account
    {code}
    *Summary:* Get driver profile
    *Description:*


    h4. Parameters







    h4. Responses
        *Status Code:* 200
        *Message:*     OK
        {code:title=Response Type}
JSend
        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "OK",
  "schema" : {
    "$ref" : "#/definitions/JSend"
  }
}
        {code}
        *Status Code:* 401
        *Message:*     Unauthorized
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Unauthorized"
}
        {code}
        *Status Code:* 403
        *Message:*     Forbidden
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Forbidden"
}
        {code}
        *Status Code:* 404
        *Message:*     Not Found
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Not Found"
}
        {code}
    ----

    h3. getDriverLocationUsingGET
    {status:colour=Yellow|title=get|subtle=false}
    {code}
    get /api/v1/driver/{driverId}/location
    {code}
    *Summary:* getDriverLocation
    *Description:*


    h4. Parameters
        h5. Path Parameters
        ||Name||Description||Required||Default||Pattern||
        |driverId |driverId |(/) | |  |








    h4. Responses
        *Status Code:* 200
        *Message:*     OK
        {code:title=Response Type}
JSendOfUserLocationDTO
        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "OK",
  "schema" : {
    "$ref" : "#/definitions/JSendOfUserLocationDTO"
  }
}
        {code}
        *Status Code:* 401
        *Message:*     Unauthorized
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Unauthorized"
}
        {code}
        *Status Code:* 403
        *Message:*     Forbidden
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Forbidden"
}
        {code}
        *Status Code:* 404
        *Message:*     Not Found
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Not Found"
}
        {code}
    ----

    h3. getDriversListByCurrentDriverUsingGET
    {status:colour=Yellow|title=get|subtle=false}
    {code}
    get /api/v1/driver/drivers
    {code}
    *Summary:* getDriversListByCurrentDriver
    *Description:*


    h4. Parameters



        h5. Query Parameters
        ||Name||Description||Required||Default||Pattern||
        |codStatus |The COD status |(x) | |  |

|fromDate | |(x) | |  |

|marketplaceId | |(x) | |  |

|marketplaceIds | |(x) | |  |

|orderBy |The field name based on which the results are ordered |(x) | |  |

|orderByDirection |The order of sorting, available values are &#39;asc&#39; and &#39;desc&#39; |(x) | |  |

|orderSize |Order Size |(x) | |  |

|page |The page number, by default it is set to 0 |(x) | |  |

|paymentType |Payment Type |(x) | |  |

|search |The Search Key filter |(x) | |  |

|searchForQuery | |(x) | |  |

|size |The size of the page, by default it is set to 20, max value 200 |(x) | |  |

|status |The comma delimited list of status values |(x) | |  |

|toDate | |(x) | |  |

|useSolr |The result will be fetched from solr instead of DB |(x) | |  |





    h4. Responses
        *Status Code:* 200
        *Message:*     OK
        {code:title=Response Type}
JSendOfSupplierDriversDTO
        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "OK",
  "schema" : {
    "$ref" : "#/definitions/JSendOfSupplierDriversDTO"
  }
}
        {code}
        *Status Code:* 401
        *Message:*     Unauthorized
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Unauthorized"
}
        {code}
        *Status Code:* 403
        *Message:*     Forbidden
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Forbidden"
}
        {code}
        *Status Code:* 404
        *Message:*     Not Found
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Not Found"
}
        {code}
    ----

    h3. getStatusMessagesUsingGET
    {status:colour=Yellow|title=get|subtle=false}
    {code}
    get /api/v1/driver/status/messages
    {code}
    *Summary:* Get status messages
    *Description:*


    h4. Parameters







    h4. Responses
        *Status Code:* 200
        *Message:*     OK
        {code:title=Response Type}
JSend
        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "OK",
  "schema" : {
    "$ref" : "#/definitions/JSend"
  }
}
        {code}
        *Status Code:* 401
        *Message:*     Unauthorized
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Unauthorized"
}
        {code}
        *Status Code:* 403
        *Message:*     Forbidden
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Forbidden"
}
        {code}
        *Status Code:* 404
        *Message:*     Not Found
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Not Found"
}
        {code}
    ----

    h3. registerAccountUsingPOST
    {status:colour=Yellow|title=post|subtle=false}
    {code}
    post /api/v1/driver/register
    {code}
    *Summary:* registerAccount
    *Description:*


    h4. Parameters

        h5. Body Parameter
        ||Name||Description||Required||Default||Pattern||
        |driverDTO |driverDTO |(/) | |  |







    h4. Responses
        *Status Code:* 200
        *Message:*     OK
        {code:title=Response Type}
JSendOfDriverDTO
        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "OK",
  "schema" : {
    "$ref" : "#/definitions/JSendOfDriverDTO"
  }
}
        {code}
        *Status Code:* 201
        *Message:*     Created
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Created"
}
        {code}
        *Status Code:* 401
        *Message:*     Unauthorized
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Unauthorized"
}
        {code}
        *Status Code:* 403
        *Message:*     Forbidden
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Forbidden"
}
        {code}
        *Status Code:* 404
        *Message:*     Not Found
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Not Found"
}
        {code}
    ----

    h3. registerDeviceUsingPOST
    {status:colour=Yellow|title=post|subtle=false}
    {code}
    post /api/v1/driver/register_device
    {code}
    *Summary:* registerDevice
    *Description:*


    h4. Parameters

        h5. Body Parameter
        ||Name||Description||Required||Default||Pattern||
        |deviceDTO |deviceDTO |(/) | |  |







    h4. Responses
        *Status Code:* 200
        *Message:*     OK
        {code:title=Response Type}
JSend
        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "OK",
  "schema" : {
    "$ref" : "#/definitions/JSend"
  }
}
        {code}
        *Status Code:* 201
        *Message:*     Created
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Created"
}
        {code}
        *Status Code:* 401
        *Message:*     Unauthorized
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Unauthorized"
}
        {code}
        *Status Code:* 403
        *Message:*     Forbidden
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Forbidden"
}
        {code}
        *Status Code:* 404
        *Message:*     Not Found
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Not Found"
}
        {code}
    ----

    h3. transferUsingPOST
    {status:colour=Yellow|title=post|subtle=false}
    {code}
    post /api/v1/driver/{id}/transfer
    {code}
    *Summary:* transfer
    *Description:*


    h4. Parameters
        h5. Path Parameters
        ||Name||Description||Required||Default||Pattern||
        |id |id |(/) | |  |




        h5. Query Parameters
        ||Name||Description||Required||Default||Pattern||
        |both |both |(x) |true |  |

|supplierId |supplierId |(/) | |  |





    h4. Responses
        *Status Code:* 200
        *Message:*     OK
        {code:title=Response Type}
JSend
        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "OK",
  "schema" : {
    "$ref" : "#/definitions/JSend"
  }
}
        {code}
        *Status Code:* 201
        *Message:*     Created
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Created"
}
        {code}
        *Status Code:* 401
        *Message:*     Unauthorized
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Unauthorized"
}
        {code}
        *Status Code:* 403
        *Message:*     Forbidden
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Forbidden"
}
        {code}
        *Status Code:* 404
        *Message:*     Not Found
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Not Found"
}
        {code}
    ----

    h3. updateAccountUsingPUT
    {status:colour=Yellow|title=put|subtle=false}
    {code}
    put /api/v1/driver/register
    {code}
    *Summary:* updateAccount
    *Description:*


    h4. Parameters

        h5. Body Parameter
        ||Name||Description||Required||Default||Pattern||
        |driverDTO |driverDTO |(/) | |  |







    h4. Responses
        *Status Code:* 200
        *Message:*     OK
        {code:title=Response Type}
JSendOfDriverDTO
        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "OK",
  "schema" : {
    "$ref" : "#/definitions/JSendOfDriverDTO"
  }
}
        {code}
        *Status Code:* 201
        *Message:*     Created
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Created"
}
        {code}
        *Status Code:* 401
        *Message:*     Unauthorized
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Unauthorized"
}
        {code}
        *Status Code:* 403
        *Message:*     Forbidden
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Forbidden"
}
        {code}
        *Status Code:* 404
        *Message:*     Not Found
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Not Found"
}
        {code}
    ----

    h3. updateDriverAttendanceDataUsingPUT
    {status:colour=Yellow|title=put|subtle=false}
    {code}
    put /api/v1/driver/check_in/update
    {code}
    *Summary:* updateDriverAttendanceData
    *Description:*


    h4. Parameters

        h5. Body Parameter
        ||Name||Description||Required||Default||Pattern||
        |driverAttendanceBatchUpdateDTO |driverAttendanceBatchUpdateDTO |(/) | |  |







    h4. Responses
        *Status Code:* 200
        *Message:*     OK
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "OK"
}
        {code}
        *Status Code:* 201
        *Message:*     Created
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Created"
}
        {code}
        *Status Code:* 401
        *Message:*     Unauthorized
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Unauthorized"
}
        {code}
        *Status Code:* 403
        *Message:*     Forbidden
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Forbidden"
}
        {code}
        *Status Code:* 404
        *Message:*     Not Found
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Not Found"
}
        {code}
    ----

    h3. updateDriverAttendanceNoteUsingPUT
    {status:colour=Yellow|title=put|subtle=false}
    {code}
    put /api/v1/driver/check_in/note
    {code}
    *Summary:* updateDriverAttendanceNote
    *Description:*


    h4. Parameters

        h5. Body Parameter
        ||Name||Description||Required||Default||Pattern||
        |driverAttendanceBatchUpdateDTO |driverAttendanceBatchUpdateDTO |(/) | |  |







    h4. Responses
        *Status Code:* 200
        *Message:*     OK
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "OK"
}
        {code}
        *Status Code:* 201
        *Message:*     Created
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Created"
}
        {code}
        *Status Code:* 401
        *Message:*     Unauthorized
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Unauthorized"
}
        {code}
        *Status Code:* 403
        *Message:*     Forbidden
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Forbidden"
}
        {code}
        *Status Code:* 404
        *Message:*     Not Found
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Not Found"
}
        {code}
    ----

    h3. updateDriverLocationUsingPOST
    {status:colour=Yellow|title=post|subtle=false}
    {code}
    post /api/v1/driver/location
    {code}
    *Summary:* updateDriverLocation
    *Description:*


    h4. Parameters

        h5. Body Parameter
        ||Name||Description||Required||Default||Pattern||
        |locationDTO |locationDTO |(/) | |  |







    h4. Responses
        *Status Code:* 200
        *Message:*     OK
        {code:title=Response Type}
JSend
        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "OK",
  "schema" : {
    "$ref" : "#/definitions/JSend"
  }
}
        {code}
        *Status Code:* 201
        *Message:*     Created
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Created"
}
        {code}
        *Status Code:* 401
        *Message:*     Unauthorized
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Unauthorized"
}
        {code}
        *Status Code:* 403
        *Message:*     Forbidden
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Forbidden"
}
        {code}
        *Status Code:* 404
        *Message:*     Not Found
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Not Found"
}
        {code}
    ----

    h3. updateDriverUsingPUT
    {status:colour=Yellow|title=put|subtle=false}
    {code}
    put /api/v1/driver/update
    {code}
    *Summary:* updateDriver
    *Description:*


    h4. Parameters

        h5. Body Parameter
        ||Name||Description||Required||Default||Pattern||
        |drivers |drivers |(/) | |  |







    h4. Responses
        *Status Code:* 200
        *Message:*     OK
        {code:title=Response Type}
JSendOfDriverDTO
        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "OK",
  "schema" : {
    "$ref" : "#/definitions/JSendOfDriverDTO"
  }
}
        {code}
        *Status Code:* 201
        *Message:*     Created
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Created"
}
        {code}
        *Status Code:* 401
        *Message:*     Unauthorized
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Unauthorized"
}
        {code}
        *Status Code:* 403
        *Message:*     Forbidden
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Forbidden"
}
        {code}
        *Status Code:* 404
        *Message:*     Not Found
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Not Found"
}
        {code}
    ----

    h3. updateSettingsUsingPUT
    {status:colour=Yellow|title=put|subtle=false}
    {code}
    put /api/v1/driver/settings
    {code}
    *Summary:* updateSettings
    *Description:*


    h4. Parameters

        h5. Body Parameter
        ||Name||Description||Required||Default||Pattern||
        |settingsDto |settingsDto |(/) | |  |







    h4. Responses
        *Status Code:* 200
        *Message:*     OK
        {code:title=Response Type}
JSend
        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "OK",
  "schema" : {
    "$ref" : "#/definitions/JSend"
  }
}
        {code}
        *Status Code:* 201
        *Message:*     Created
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Created"
}
        {code}
        *Status Code:* 401
        *Message:*     Unauthorized
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Unauthorized"
}
        {code}
        *Status Code:* 403
        *Message:*     Forbidden
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Forbidden"
}
        {code}
        *Status Code:* 404
        *Message:*     Not Found
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Not Found"
}
        {code}
    ----

    h3. driverUpdateJobUsingPUT
    {status:colour=Yellow|title=put|subtle=false}
    {code}
    put /api/v1/driver/job/{id}
    {code}
    *Summary:* driverUpdateJob
    *Description:*


    h4. Parameters
        h5. Path Parameters
        ||Name||Description||Required||Default||Pattern||
        |id |The unique ID which was assigned to the Job |(/) | |  |


        h5. Body Parameter
        ||Name||Description||Required||Default||Pattern||
        |jobUpdateDTO |jobUpdateDTO |(/) | |  |







    h4. Responses
        *Status Code:* 200
        *Message:*     OK
        {code:title=Response Type}
JSendOfOrderDTO
        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "OK",
  "schema" : {
    "$ref" : "#/definitions/JSendOfOrderDTO"
  }
}
        {code}
        *Status Code:* 201
        *Message:*     Created
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Created"
}
        {code}
        *Status Code:* 401
        *Message:*     Unauthorized
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Unauthorized"
}
        {code}
        *Status Code:* 403
        *Message:*     Forbidden
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Forbidden"
}
        {code}
        *Status Code:* 404
        *Message:*     Not Found
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Not Found"
}
        {code}
    ----

    h3. getJobOrdersUsingGET
    {status:colour=Yellow|title=get|subtle=false}
    {code}
    get /api/v1/driver/job_orders/{job_id}
    {code}
    *Summary:* Get job orders
    *Description:* Get job orders


    h4. Parameters
        h5. Path Parameters
        ||Name||Description||Required||Default||Pattern||
        |jobId |job_id |(/) | |  |








    h4. Responses
        *Status Code:* 200
        *Message:*     OK
        {code:title=Response Type}
JSendOfTableListOfOrderDTO
        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "OK",
  "schema" : {
    "$ref" : "#/definitions/JSendOfTableListOfOrderDTO"
  }
}
        {code}
        *Status Code:* 401
        *Message:*     Unauthorized
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Unauthorized"
}
        {code}
        *Status Code:* 403
        *Message:*     Forbidden
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Forbidden"
}
        {code}
        *Status Code:* 404
        *Message:*     Not Found
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Not Found"
}
        {code}
    ----

    h3. batchUpdateStatusUsingPOST
    {status:colour=Yellow|title=post|subtle=false}
    {code}
    post /api/v1/driver/order/batch_update_status
    {code}
    *Summary:* Batch Update Status by Order Numbers
    *Description:*


    h4. Parameters

        h5. Body Parameter
        ||Name||Description||Required||Default||Pattern||
        |batchOrderDto |batchOrderDto |(/) | |  |







    h4. Responses
        *Status Code:* 200
        *Message:*     OK
        {code:title=Response Type}
JSend
        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "OK",
  "schema" : {
    "$ref" : "#/definitions/JSend"
  }
}
        {code}
        *Status Code:* 201
        *Message:*     Created
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Created"
}
        {code}
        *Status Code:* 401
        *Message:*     Unauthorized
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Unauthorized"
}
        {code}
        *Status Code:* 403
        *Message:*     Forbidden
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Forbidden"
}
        {code}
        *Status Code:* 404
        *Message:*     Not Found
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Not Found"
}
        {code}
    ----

    h3. driverAddNoteUsingPOST
    {status:colour=Yellow|title=post|subtle=false}
    {code}
    post /api/v1/driver/order/{id}/note
    {code}
    *Summary:* Add Public Order Note by Order ID
    *Description:* Add a Public Order Note by the Order ID.


    h4. Parameters
        h5. Path Parameters
        ||Name||Description||Required||Default||Pattern||
        |id |The unique ID which was assigned to the Order |(/) | |  |


        h5. Body Parameter
        ||Name||Description||Required||Default||Pattern||
        |note |Object that holds a note data |(/) | |  |







    h4. Responses
        *Status Code:* 200
        *Message:*     OK
        {code:title=Response Type}
JSend
        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "OK",
  "schema" : {
    "$ref" : "#/definitions/JSend"
  }
}
        {code}
        *Status Code:* 201
        *Message:*     Created
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Created"
}
        {code}
        *Status Code:* 401
        *Message:*     Unauthorized
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Unauthorized"
}
        {code}
        *Status Code:* 403
        *Message:*     Forbidden
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Forbidden"
}
        {code}
        *Status Code:* 404
        *Message:*     Not Found
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Not Found"
}
        {code}
    ----

    h3. driverChangeStatusUsingPUT
    {status:colour=Yellow|title=put|subtle=false}
    {code}
    put /api/v1/driver/order/{id}/status
    {code}
    *Summary:* driverChangeStatus
    *Description:*


    h4. Parameters
        h5. Path Parameters
        ||Name||Description||Required||Default||Pattern||
        |id |id |(/) | |  |


        h5. Body Parameter
        ||Name||Description||Required||Default||Pattern||
        |statusDto |statusDto |(/) | |  |







    h4. Responses
        *Status Code:* 200
        *Message:*     OK
        {code:title=Response Type}
JSendOfOrderDTO
        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "OK",
  "schema" : {
    "$ref" : "#/definitions/JSendOfOrderDTO"
  }
}
        {code}
        *Status Code:* 201
        *Message:*     Created
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Created"
}
        {code}
        *Status Code:* 401
        *Message:*     Unauthorized
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Unauthorized"
}
        {code}
        *Status Code:* 403
        *Message:*     Forbidden
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Forbidden"
}
        {code}
        *Status Code:* 404
        *Message:*     Not Found
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Not Found"
}
        {code}
    ----

    h3. driverJobOrdersReceivePaymentUsingPUT
    {status:colour=Yellow|title=put|subtle=false}
    {code}
    put /api/v1/driver/job_orders/receive_payment
    {code}
    *Summary:* driverJobOrdersReceivePayment
    *Description:*


    h4. Parameters

        h5. Body Parameter
        ||Name||Description||Required||Default||Pattern||
        |chargeItems |chargeItems |(/) | |  |







    h4. Responses
        *Status Code:* 200
        *Message:*     OK
        {code:title=Response Type}
JSend
        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "OK",
  "schema" : {
    "$ref" : "#/definitions/JSend"
  }
}
        {code}
        *Status Code:* 201
        *Message:*     Created
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Created"
}
        {code}
        *Status Code:* 401
        *Message:*     Unauthorized
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Unauthorized"
}
        {code}
        *Status Code:* 403
        *Message:*     Forbidden
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Forbidden"
}
        {code}
        *Status Code:* 404
        *Message:*     Not Found
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Not Found"
}
        {code}
    ----

    h3. driverReceivePaymentUsingPUT
    {status:colour=Yellow|title=put|subtle=false}
    {code}
    put /api/v1/driver/order/{order_id}/receive_payment
    {code}
    *Summary:* driverReceivePayment
    *Description:*


    h4. Parameters
        h5. Path Parameters
        ||Name||Description||Required||Default||Pattern||
        |orderId |order_id |(/) | |  |


        h5. Body Parameter
        ||Name||Description||Required||Default||Pattern||
        |chargeItems |chargeItems |(/) | |  |







    h4. Responses
        *Status Code:* 200
        *Message:*     OK
        {code:title=Response Type}
JSend
        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "OK",
  "schema" : {
    "$ref" : "#/definitions/JSend"
  }
}
        {code}
        *Status Code:* 201
        *Message:*     Created
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Created"
}
        {code}
        *Status Code:* 401
        *Message:*     Unauthorized
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Unauthorized"
}
        {code}
        *Status Code:* 403
        *Message:*     Forbidden
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Forbidden"
}
        {code}
        *Status Code:* 404
        *Message:*     Not Found
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Not Found"
}
        {code}
    ----

    h3. driverSignatureUsingPUT
    {status:colour=Yellow|title=put|subtle=false}
    {code}
    put /api/v1/driver/order/{orderId}/signature
    {code}
    *Summary:* driverSignature
    *Description:*


    h4. Parameters
        h5. Path Parameters
        ||Name||Description||Required||Default||Pattern||
        |orderId |orderId |(/) | |  |


        h5. Body Parameter
        ||Name||Description||Required||Default||Pattern||
        |orderSignatureDTO |orderSignatureDTO |(/) | |  |







    h4. Responses
        *Status Code:* 200
        *Message:*     OK
        {code:title=Response Type}
JSend
        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "OK",
  "schema" : {
    "$ref" : "#/definitions/JSend"
  }
}
        {code}
        *Status Code:* 201
        *Message:*     Created
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Created"
}
        {code}
        *Status Code:* 401
        *Message:*     Unauthorized
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Unauthorized"
}
        {code}
        *Status Code:* 403
        *Message:*     Forbidden
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Forbidden"
}
        {code}
        *Status Code:* 404
        *Message:*     Not Found
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Not Found"
}
        {code}
    ----

    h3. getCancellationReasonsUsingGET
    {status:colour=Yellow|title=get|subtle=false}
    {code}
    get /api/v1/driver/cancellation_reasons/{order_status}
    {code}
    *Summary:* getCancellationReasons
    *Description:*


    h4. Parameters
        h5. Path Parameters
        ||Name||Description||Required||Default||Pattern||
        |orderStatus |order_status |(/) | |  |








    h4. Responses
        *Status Code:* 200
        *Message:*     OK
        {code:title=Response Type}
JSendOfListOfstring
        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "OK",
  "schema" : {
    "$ref" : "#/definitions/JSendOfListOfstring"
  }
}
        {code}
        *Status Code:* 401
        *Message:*     Unauthorized
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Unauthorized"
}
        {code}
        *Status Code:* 403
        *Message:*     Forbidden
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Forbidden"
}
        {code}
        *Status Code:* 404
        *Message:*     Not Found
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Not Found"
}
        {code}
    ----

    h3. getDriverOrderUsingGET
    {status:colour=Yellow|title=get|subtle=false}
    {code}
    get /api/v1/driver/order/{id}
    {code}
    *Summary:* getDriverOrder
    *Description:*


    h4. Parameters
        h5. Path Parameters
        ||Name||Description||Required||Default||Pattern||
        |id |id |(/) | |  |








    h4. Responses
        *Status Code:* 200
        *Message:*     OK
        {code:title=Response Type}
JSendOfOrderDTO
        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "OK",
  "schema" : {
    "$ref" : "#/definitions/JSendOfOrderDTO"
  }
}
        {code}
        *Status Code:* 401
        *Message:*     Unauthorized
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Unauthorized"
}
        {code}
        *Status Code:* 403
        *Message:*     Forbidden
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Forbidden"
}
        {code}
        *Status Code:* 404
        *Message:*     Not Found
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Not Found"
}
        {code}
    ----

    h3. getDriverOrdersUsingGET
    {status:colour=Yellow|title=get|subtle=false}
    {code}
    get /api/v1/driver/orders
    {code}
    *Summary:* Get driver orders by status
    *Description:*


    h4. Parameters



        h5. Query Parameters
        ||Name||Description||Required||Default||Pattern||
        |codStatus |The COD status |(x) | |  |

|fromDate | |(x) | |  |

|marketplaceId | |(x) | |  |

|marketplaceIds | |(x) | |  |

|orderBy |The field name based on which the results are ordered |(x) | |  |

|orderByDirection |The order of sorting, available values are &#39;asc&#39; and &#39;desc&#39; |(x) | |  |

|orderSize |Order Size |(x) | |  |

|page |The page number, by default it is set to 0 |(x) | |  |

|paymentType |Payment Type |(x) | |  |

|search |The Search Key filter |(x) | |  |

|searchForQuery | |(x) | |  |

|size |The size of the page, by default it is set to 20, max value 200 |(x) | |  |

|status |The comma delimited list of status values |(x) | |  |

|toDate | |(x) | |  |

|useSolr |Use Solr |(x) | |  |





    h4. Responses
        *Status Code:* 200
        *Message:*     OK
        {code:title=Response Type}
JSendOfTableListOfOrderDTO
        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "OK",
  "schema" : {
    "$ref" : "#/definitions/JSendOfTableListOfOrderDTO"
  }
}
        {code}
        *Status Code:* 401
        *Message:*     Unauthorized
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Unauthorized"
}
        {code}
        *Status Code:* 403
        *Message:*     Forbidden
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Forbidden"
}
        {code}
        *Status Code:* 404
        *Message:*     Not Found
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Not Found"
}
        {code}
    ----

    h3. getNotesForDriverUsingGET
    {status:colour=Yellow|title=get|subtle=false}
    {code}
    get /api/v1/driver/order/{id}/notes
    {code}
    *Summary:* getNotesForDriver
    *Description:*


    h4. Parameters
        h5. Path Parameters
        ||Name||Description||Required||Default||Pattern||
        |id |id |(/) | |  |




        h5. Query Parameters
        ||Name||Description||Required||Default||Pattern||
        |fromDate | |(x) | |  |

|marketplaceId | |(x) | |  |

|marketplaceIds | |(x) | |  |

|orderId |Order Id |(x) | |  |

|orderBy |The field name based on which the results are ordered |(x) | |  |

|orderByDirection |The order of sorting, available values are &#39;asc&#39; and &#39;desc&#39; |(x) | |  |

|page |The page number, by default it is set to 0 |(x) | |  |

|privacy |Privacy |(x) | |  |

|role | |(x) | |  |

|search |The Search Key filter |(x) | |  |

|searchForQuery | |(x) | |  |

|size |The size of the page, by default it is set to 20, max value 200 |(x) | |  |

|toDate | |(x) | |  |

|useSolr |The result will be fetched from solr instead of DB |(x) | |  |





    h4. Responses
        *Status Code:* 200
        *Message:*     OK
        {code:title=Response Type}
JSendOfTableListOfNoteDTO
        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "OK",
  "schema" : {
    "$ref" : "#/definitions/JSendOfTableListOfNoteDTO"
  }
}
        {code}
        *Status Code:* 401
        *Message:*     Unauthorized
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Unauthorized"
}
        {code}
        *Status Code:* 403
        *Message:*     Forbidden
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Forbidden"
}
        {code}
        *Status Code:* 404
        *Message:*     Not Found
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Not Found"
}
        {code}
    ----

    h3. getOrderByBarcodeUsingGET
    {status:colour=Yellow|title=get|subtle=false}
    {code}
    get /api/v1/driver/order/barcode/{barcode}
    {code}
    *Summary:* Get order with barcode from system
    *Description:*


    h4. Parameters
        h5. Path Parameters
        ||Name||Description||Required||Default||Pattern||
        |barcode |barcode |(/) | |  |








    h4. Responses
        *Status Code:* 200
        *Message:*     OK
        {code:title=Response Type}
JSendOfOrderDTO
        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "OK",
  "schema" : {
    "$ref" : "#/definitions/JSendOfOrderDTO"
  }
}
        {code}
        *Status Code:* 401
        *Message:*     Unauthorized
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Unauthorized"
}
        {code}
        *Status Code:* 403
        *Message:*     Forbidden
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Forbidden"
}
        {code}
        *Status Code:* 404
        *Message:*     Not Found
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Not Found"
}
        {code}
    ----

    h3. hasActiveOrdersUsingGET
    {status:colour=Yellow|title=get|subtle=false}
    {code}
    get /api/v1/driver/order/has_active
    {code}
    *Summary:* hasActiveOrders
    *Description:*


    h4. Parameters



        h5. Query Parameters
        ||Name||Description||Required||Default||Pattern||
        |status |status |(/) | |  |





    h4. Responses
        *Status Code:* 200
        *Message:*     OK
        {code:title=Response Type}
JSend
        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "OK",
  "schema" : {
    "$ref" : "#/definitions/JSend"
  }
}
        {code}
        *Status Code:* 401
        *Message:*     Unauthorized
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Unauthorized"
}
        {code}
        *Status Code:* 403
        *Message:*     Forbidden
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Forbidden"
}
        {code}
        *Status Code:* 404
        *Message:*     Not Found
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Not Found"
}
        {code}
    ----

    h3. requestRecipientLocationUsingGET
    {status:colour=Yellow|title=get|subtle=false}
    {code}
    get /api/v1/driver/order/{order_id}/recipient/location
    {code}
    *Summary:* Request recipient location
    *Description:*


    h4. Parameters
        h5. Path Parameters
        ||Name||Description||Required||Default||Pattern||
        |orderId |order_id |(/) | |  |








    h4. Responses
        *Status Code:* 200
        *Message:*     OK
        {code:title=Response Type}
JSend
        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "OK",
  "schema" : {
    "$ref" : "#/definitions/JSend"
  }
}
        {code}
        *Status Code:* 401
        *Message:*     Unauthorized
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Unauthorized"
}
        {code}
        *Status Code:* 403
        *Message:*     Forbidden
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Forbidden"
}
        {code}
        *Status Code:* 404
        *Message:*     Not Found
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Not Found"
}
        {code}
    ----

    h3. updateFetchItemUsingPUT
    {status:colour=Yellow|title=put|subtle=false}
    {code}
    put /api/v1/driver/order/{id}/fetch_item
    {code}
    *Summary:* updateFetchItem
    *Description:*


    h4. Parameters
        h5. Path Parameters
        ||Name||Description||Required||Default||Pattern||
        |id |id |(/) | |  |


        h5. Body Parameter
        ||Name||Description||Required||Default||Pattern||
        |fetchItemDTO |fetchItemDTO |(/) | |  |







    h4. Responses
        *Status Code:* 200
        *Message:*     OK
        {code:title=Response Type}
JSend
        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "OK",
  "schema" : {
    "$ref" : "#/definitions/JSend"
  }
}
        {code}
        *Status Code:* 201
        *Message:*     Created
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Created"
}
        {code}
        *Status Code:* 401
        *Message:*     Unauthorized
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Unauthorized"
}
        {code}
        *Status Code:* 403
        *Message:*     Forbidden
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Forbidden"
}
        {code}
        *Status Code:* 404
        *Message:*     Not Found
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Not Found"
}
        {code}
    ----

    h3. updateOrderBarcodeUsingPUT
    {status:colour=Yellow|title=put|subtle=false}
    {code}
    put /api/v1/driver/order/{orderId}/barcode
    {code}
    *Summary:* updateOrderBarcode
    *Description:*


    h4. Parameters
        h5. Path Parameters
        ||Name||Description||Required||Default||Pattern||
        |orderId |orderId |(/) | |  |




        h5. Query Parameters
        ||Name||Description||Required||Default||Pattern||
        |barcode |barcode |(/) | |  |

|barcodeType |barcodeType |(/) | |  |





    h4. Responses
        *Status Code:* 200
        *Message:*     OK
        {code:title=Response Type}
JSend
        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "OK",
  "schema" : {
    "$ref" : "#/definitions/JSend"
  }
}
        {code}
        *Status Code:* 201
        *Message:*     Created
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Created"
}
        {code}
        *Status Code:* 401
        *Message:*     Unauthorized
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Unauthorized"
}
        {code}
        *Status Code:* 403
        *Message:*     Forbidden
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Forbidden"
}
        {code}
        *Status Code:* 404
        *Message:*     Not Found
        {code:title=Response Type}

        {code}
        See [#models]



        {code:title=Response Schema |collapse=true}
{
  "description" : "Not Found"
}
        {code}
    ----

h2. Models

        h3. AddNoteDTO
        ||Field Name||Required||Type||Description||
         |cancellation_reason | |String | |
 |content | |String | |
 |inquiries | |String | |
 |privacy | |String | |
 |reason | |String | |
        h3. BarcodeDTO
        ||Field Name||Required||Type||Description||
         |barcode | |String | |
 |id | |Long | |
 |type | |String | |
        h3. Batch_order
        ||Field Name||Required||Type||Description||
         |driver | |UserItem | |
 |event_date | |String | |
 |ignore_nsa | |Boolean | |
 |marketplace_id | |Long | |
 |note | |String | |
 |order_numbers | |array[String] | |
 |order_signature | |OrderSignatureDTO | |
 |order_status | |String | |
 |paid_to_customer | |Boolean | |
 |paid_to_wing | |Boolean | |
 |privacy | |String | |
 |reason | |String | |
 |requires_attention | |Boolean | |
 |scheduled_for_cancellation | |Boolean | |
 |signature | |String | |
 |supplier | |UserItem | |
 |transit_mode | |String | |
 |warehouse | |SelectItem | |
        h3. CallTimingsDTO
        ||Field Name||Required||Type||Description||
         |address_type | |String | |
 |call_timing_permission_type | |String | |
 |courier_type | |String | |
 |customer_id | |Long | |
 |end_time | |String | |
 |id | |Long | |
 |start_time | |String | |
        h3. Charge_item
        ||Field Name||Required||Type||Description||
         |base_currency | |CurrencyDTO | |
 |charge_type | |String | |
 |currency | |CurrencyDTO | |
 |exchange_rate | |BigDecimal | |
 |refund | |Boolean | |
 |id | |Long | |
 |quantity | |Integer | |
 |charge | |BigDecimal | |
 |date | |String | |
 |paid | |Boolean | |
 |payer | |String | |
 |paid_to_customer | |Boolean | |
 |paid_to_wing | |Boolean | |
        h3. CurrencyDTO
        ||Field Name||Required||Type||Description||
         |code | |String | |
 |name | |String | |
        h3. CustomerSettingsDTO
        ||Field Name||Required||Type||Description||
         |push_status | |Boolean | |
 |sms_status | |Boolean | |
 |marketplace_id | |Long | |
        h3. DeviceDTO
        ||Field Name||Required||Type||Description||
         |app_version | |String | |
 |device_type | |String | |
 |device_uuid | |String | |
 |reg_id | |String | |
        h3. Direction_data
        ||Field Name||Required||Type||Description||
         |path | |String | |
 |distance | |text_value | |
 |duration | |text_value | |
        h3. DriverAttendanceBatchUpdateDTO
        ||Field Name||Required||Type||Description||
         |ids | |array[Long] | |
 |note | |String | |
 |type | |String | |
        h3. DriverDTO
        ||Field Name||Required||Type||Description||
         |activated | |Boolean | |
 |authorities | |array[String] | |
 |birth_date | |String | |
 |bonus | |BigDecimal | |
 |company_trade_license | |String | |
 |country | |SelectItem | |
 |created_date | |String | |
 |currency | |CurrencyDTO | |
 |dedicated | |Boolean | |
 |dispatchable | |Boolean | |
 |driver_id | |Long | |
 |email | |String | |
 |emirates_id_back | |String | |
 |emirates_id_front | |String | |
 |first_name | |String | |
 |full_name | |String | |
 |gender | |String | |
 |languages | |String | |
 |last_name | |String | |
 |license_image | |String | |
 |login | |String | |
 |marketplace_ids | |array[Long] | |
 |parent_supplier | |SelectItem | |
 |password | |String | |
 |phone | |String | |
 |photo | |String | |
 |push_status | |Boolean | |
 |rate | |Float | |
 |rta_card | |String | |
 |sanction_cancellation_reason | |String | |
 |sanction_reason | |String | |
 |sms_status | |Boolean | |
 |start_date_as_dedicated | |String | |
 |status | |String | |
 |supplier | |UserItem | |
 |user_id | |Long | |
 |valid_phone | |Boolean | |
 |vehicle | |VehicleDTO | |
 |version | |Integer | |
 |warehouse | |SelectItem | |
 |marketplace_id | |Long | |
        h3. Fetch_item
        ||Field Name||Required||Type||Description||
         |actual_description | |String | |
 |actual_name | |String | |
 |actual_photo | |String | |
 |actual_price | |BigDecimal | |
 |approx_price | |BigDecimal | |
 |currency | |CurrencyDTO | |
 |desc | |String | |
 |id | |Long | |
 |match_type | |String | |
 |message | |String | |
 |name | |String | |
 |paid | |Boolean | |
 |photos | |array[String] | |
 |shop_name | |String | |
 |status | |String | |
        h3. JSend
        ||Field Name||Required||Type||Description||
         |code | |String | |
 |data | |Object | |
 |detail | |String | |
 |instance | |URI | |
 |message | |String | |
 |status | |String | |
 |title | |String | |
 |type | |URI | |
        h3. JSendOfDriverDTO
        ||Field Name||Required||Type||Description||
         |code | |String | |
 |data | |DriverDTO | |
 |detail | |String | |
 |instance | |URI | |
 |message | |String | |
 |status | |String | |
 |title | |String | |
 |type | |URI | |
        h3. JSendOfListOfCallTimingsDTO
        ||Field Name||Required||Type||Description||
         |code | |String | |
 |data | |array[CallTimingsDTO] | |
 |detail | |String | |
 |instance | |URI | |
 |message | |String | |
 |status | |String | |
 |title | |String | |
 |type | |URI | |
        h3. JSendOfListOfstring
        ||Field Name||Required||Type||Description||
         |code | |String | |
 |data | |array[String] | |
 |detail | |String | |
 |instance | |URI | |
 |message | |String | |
 |status | |String | |
 |title | |String | |
 |type | |URI | |
        h3. JSendOfOrderDTO
        ||Field Name||Required||Type||Description||
         |code | |String | |
 |data | |OrderDTO | |
 |detail | |String | |
 |instance | |URI | |
 |message | |String | |
 |status | |String | |
 |title | |String | |
 |type | |URI | |
        h3. JSendOfSelectItem
        ||Field Name||Required||Type||Description||
         |code | |String | |
 |data | |SelectItem | |
 |detail | |String | |
 |instance | |URI | |
 |message | |String | |
 |status | |String | |
 |title | |String | |
 |type | |URI | |
        h3. JSendOfSupplierDriversDTO
        ||Field Name||Required||Type||Description||
         |code | |String | |
 |data | |SupplierDriversDTO | |
 |detail | |String | |
 |instance | |URI | |
 |message | |String | |
 |status | |String | |
 |title | |String | |
 |type | |URI | |
        h3. JSendOfTableListOfNoteDTO
        ||Field Name||Required||Type||Description||
         |code | |String | |
 |data | |TableListOfNoteDTO | |
 |detail | |String | |
 |instance | |URI | |
 |message | |String | |
 |status | |String | |
 |title | |String | |
 |type | |URI | |
        h3. JSendOfTableListOfOrderDTO
        ||Field Name||Required||Type||Description||
         |code | |String | |
 |data | |TableListOfOrderDTO | |
 |detail | |String | |
 |instance | |URI | |
 |message | |String | |
 |status | |String | |
 |title | |String | |
 |type | |URI | |
        h3. JSendOfTableListOfStatusMessagesDTO
        ||Field Name||Required||Type||Description||
         |code | |String | |
 |data | |TableListOfStatusMessagesDTO | |
 |detail | |String | |
 |instance | |URI | |
 |message | |String | |
 |status | |String | |
 |title | |String | |
 |type | |URI | |
        h3. JSendOfTableListOfTransactionDataDTO
        ||Field Name||Required||Type||Description||
         |code | |String | |
 |data | |TableListOfTransactionDataDTO | |
 |detail | |String | |
 |instance | |URI | |
 |message | |String | |
 |status | |String | |
 |title | |String | |
 |type | |URI | |
        h3. JSendOfTransactionListDTO
        ||Field Name||Required||Type||Description||
         |code | |String | |
 |data | |TransactionListDTO | |
 |detail | |String | |
 |instance | |URI | |
 |message | |String | |
 |status | |String | |
 |title | |String | |
 |type | |URI | |
        h3. JSendOfUserJWTToken
        ||Field Name||Required||Type||Description||
         |code | |String | |
 |data | |UserJWTToken | |
 |detail | |String | |
 |instance | |URI | |
 |message | |String | |
 |status | |String | |
 |title | |String | |
 |type | |URI | |
        h3. JSendOfUserLocationDTO
        ||Field Name||Required||Type||Description||
         |code | |String | |
 |data | |UserLocationDTO | |
 |detail | |String | |
 |instance | |URI | |
 |message | |String | |
 |status | |String | |
 |title | |String | |
 |type | |URI | |
        h3. JobUpdateDTO
        ||Field Name||Required||Type||Description||
         |driver | |UserItem | |
 |id | |Long | |
 |job_statuses | |array[OrderJobStatusDTO] | |
 |signature | |OrderSignatureDTO | |
 |status | |String | |
        h3. Location
        ||Field Name||Required||Type||Description||
         |place_location | |Boolean | |
 |lat | |Double | |
 |lon | |Double | |
 |city | |String | |
 |pickup | |Boolean | |
 |details | |String | |
 |address | |String | |
 |contact_name | |String | |
 |email | |String | |
 |phone | |String | |
 |company_name | |String | |
 |confirmed_by_recipient | |Boolean | |
 |address_type | |String | |
 |postcode | |String | |
 |address_city | |String | |
 |address_street | |String | |
 |preferred_time | |String | |
 |neighborhood | |String | |
 |location_source_type | |String | |
        h3. Login
        ||Field Name||Required||Type||Description||
         |username | |String | |
 |password | |String | |
 |remember_me | |Boolean |If set true the &#39;id_token&#39; is valid for 365 days, otherwise it expires in 30 minutes |
        h3. ManifestDTO
        ||Field Name||Required||Type||Description||
         |barcode | |String | |
 |id | |Long | |
 |type | |String | |
        h3. NoteDTO
        ||Field Name||Required||Type||Description||
         |cancellation_reason | |String | |
 |content | |String | |
 |created_date | |String | |
 |entity_class | |String | |
 |entity_id | |Long | |
 |id | |Long | |
 |inquiries | |String | |
 |noted_by | |SelectItem | |
 |noted_by_role | |String | |
 |privacy | |String | |
 |reason | |String | |
 |requires_attention | |Boolean | |
 |scheduled_for_cancellation | |Boolean | |
        h3. OrderDTO
        ||Field Name||Required||Type||Description||
         |allocated_from_warehouse | |Boolean | |
 |amount | |BigDecimal | |
 |attachments | |array[Long] | |
 |auto_cancelled | |Boolean | |
 |barcodes | |array[BarcodeDTO] | |
 |bonus | |BigDecimal | |
 |charge_items | |array[charge_item] | |
 |chargeable_weight | |BigDecimal | |
 |cod_status | |String | |
 |completed | |String | |
 |created_date | |String | |
 |currency | |CurrencyDTO | |
 |customer | |UserItem | |
 |customer_currency | |CurrencyDTO | |
 |deadline_time | |String | |
 |delivered_to | |String | |
 |delivered_to_phone | |String | |
 |delivered_to_photo | |String | |
 |delivered_to_photo_id | |Long | |
 |delivery_attempt_count | |Long | |
 |delivery_signature | |String | |
 |delivery_signature_id | |Long | |
 |delivery_status | |String | |
 |delivery_timeslot | |TimeslotDTO | |
 |delivery_timeslot_history | |TimeslotDTO | |
 |destination_warehouse | |SelectItem | |
 |device_details | |String | |
 |driver | |UserItem | |
 |estimated_delivery_time | |String | |
 |estimated_pickup_time | |String | |
 |fetch_item | |fetch_item | |
 |force_create | |Boolean | |
 |fragile | |Boolean | |
 |heavy_type | |String | |
 |id | |Long | |
 |id_card_required | |Boolean | |
 |internal_promise_date | |String | |
 |items | |array[order_item] | |
 |last_cod_status_date | |String | |
 |last_mile_driver | |UserItem | |
 |last_modified_date | |String | |
 |last_status_date | |String | |
 |location_history | |array[location] | |
 |locations | |array[location] | |
 |manifests | |array[ManifestDTO] | |
 |marketplace_ids | |array[Long] | |
 |merchant_promise_date | |String | |
 |note | |String | |
 |order_count | |Integer | |
 |order_number | |String | |
 |parcel_value | |BigDecimal | |
 |payer | |String | |
 |payment | |OrderPaymentDTO | |
 |payment_params | |PayFortDTO | |
 |payment_status | |Boolean | |
 |payment_type | |String | |
 |payment_url | |String | |
 |photos | |array[String] | |
 |pick_up_attempt_count | |Long | |
 |pick_up_driver | |UserItem | |
 |pickup_number | |String | |
 |pickup_time | |String | |
 |pickup_time_now | |Boolean | |
 |pickup_timeslot | |TimeslotDTO | |
 |pickup_timeslot_history | |TimeslotDTO | |
 |piece_count | |Integer | |
 |previous_driver | |UserItem | |
 |promo | |PromoDTO | |
 |recipient | |UserItem | |
 |recipient_not_available | |String | |
 |reference_id | |String | |
 |requires_attention | |Boolean | |
 |reviews | |array[ReviewDTO] | |
 |scanned_piece_count | |Integer | |
 |scheduled_for_cancellation | |Boolean | |
 |seller_id | |String | |
 |seller_name | |String | |
 |sender_from | |String | |
 |sender_phone | |String | |
 |sender_photo | |String | |
 |sender_photo_id | |Long | |
 |sender_signature | |String | |
 |sender_signature_id | |Long | |
 |shipment_number | |String | |
 |size | |String | |
 |status | |String | |
 |supplier | |UserItem | |
 |tracking_url | |String | |
 |type | |String | |
 |uae | |Boolean | |
 |unique_id | |String | |
 |version | |Integer | |
 |warehouse | |SelectItem | |
 |weight | |Double | |
 |package | |package_item |If package is not provided the default package set from the admin page will be assigned automatically |
        h3. OrderJobStatusDTO
        ||Field Name||Required||Type||Description||
         |order_number | |String | |
 |status | |String | |
        h3. OrderPaymentDTO
        ||Field Name||Required||Type||Description||
         |charge | |Double | |
 |currency | |String | |
 |id | |Long | |
 |order_id | |Long | |
 |payment_type | |String | |
        h3. OrderSignatureDTO
        ||Field Name||Required||Type||Description||
         |name | |String | |
 |order_id | |Long | |
 |phone | |String | |
 |photo | |String | |
 |photo_id | |Long | |
 |signature | |String | |
 |signature_id | |Long | |
 |type | |String | |
        h3. Order_item
        ||Field Name||Required||Type||Description||
         |desc | |String | |
 |id | |Long | |
 |quantity | |String | |
        h3. Order_warehouse
        ||Field Name||Required||Type||Description||
         |driver | |UserItem | |
 |event_date | |String | |
 |ignore_nsa | |Boolean | |
 |marketplace_id | |Long | |
 |note | |String | |
 |order_numbers | |array[String] | |
 |order_signature | |OrderSignatureDTO | |
 |order_status | |String | |
 |paid_to_customer | |Boolean | |
 |paid_to_wing | |Boolean | |
 |privacy | |String | |
 |reason | |String | |
 |requires_attention | |Boolean | |
 |scheduled_for_cancellation | |Boolean | |
 |supplier | |UserItem | |
 |transit_mode | |String | |
 |warehouse | |SelectItem | |
        h3. Package_item
        ||Field Name||Required||Type||Description||
         |id | |Long | |
 |name | |String | |
 |code | |String | |
 |from_city | |String | |
 |to_city | |String | |
 |capacity | |String | |
 |price | |price | |
 |courier_type | |String | |
 |courier_type_icon | |String | |
 |vehicle_type | |String | |
 |delivery_label | |String | |
 |delivery_label_helper | |String | |
 |cutoff_start | |String | |
 |cutoff_end | |String | |
 |has_cutoff_time | |Boolean | |
 |active | |Boolean | |
 |menu | |SelectItem | |
 |from_country | |SelectItem | |
 |to_country | |SelectItem | |
 |from_city_id | |Long | |
 |to_city_id | |Long | |
        h3. PayFortDTO
        ||Field Name||Required||Type||Description||
         |access_code | |String | |
 |amount | |Double | |
 |command | |String | |
 |currency | |String | |
 |customer_email | |String | |
 |customer_ip | |String | |
 |customer_name | |String | |
 |eci | |String | |
 |expiry_date | |String | |
 |fort_id | |String | |
 |language | |String | |
 |merchant_identifier | |String | |
 |merchant_reference | |String | |
 |order_id | |Long | |
 |pay_fort_amount | |Integer | |
 |payment_option | |String | |
 |payment_url | |String | |
 |refunded | |Boolean | |
 |response_code | |String | |
 |response_message | |String | |
 |return_url | |String | |
 |sdk_token | |String | |
 |signature | |String | |
 |status | |String | |
        h3. Price
        ||Field Name||Required||Type||Description||
         |currency | |CurrencyDTO | |
 |direction_data | |direction_data | |
 |base_rate | |Double | |
 |moving_rate | |Double | |
 |total | |BigDecimal | |
 |old_total | |BigDecimal | |
 |extra_fixed_fare | |BigDecimal | |
 |weight_rate | |Double | |
        h3. PromoDTO
        ||Field Name||Required||Type||Description||
         |benefit_type | |String | |
 |benefit_value | |BigDecimal | |
 |code | |String | |
 |count_of_used | |Integer | |
 |discount_cap | |BigDecimal | |
 |id | |Long | |
 |image | |String | |
 |is_public | |String | |
 |package_type | |String | |
 |subtitle | |String | |
 |title | |String | |
        h3. ReceiveChargeItemDTO
        ||Field Name||Required||Type||Description||
         |charge_type | |String | |
 |order_id | |Long | |
 |paid | |Boolean | |
 |payer | |String | |
        h3. ReferenceDTO
        ||Field Name||Required||Type||Description||
         |code | |String | |
 |gparent_code | |String | |
 |id | |Long | |
 |name | |String | |
 |parent_code | |String | |
        h3. ReviewDTO
        ||Field Name||Required||Type||Description||
         |customer | |UserItem | |
 |driver | |UserItem | |
 |id | |Long | |
 |note | |String | |
 |order_id | |Long | |
 |star | |Float | |
 |type | |String | |
        h3. SelectItem
        ||Field Name||Required||Type||Description||
         |description | |String | |
 |id | |Long | |
 |name | |String | |
        h3. StatusDTO
        ||Field Name||Required||Type||Description||
         |actual_delivery_option | |String | |
 |cancellation_reason | |String | |
 |driver_cancellation_note | |String | |
 |event_date | |String | |
 |payment_status | |Boolean | |
 |signature | |OrderSignatureDTO | |
 |status | |String | |
        h3. StatusMessagesDTO
        ||Field Name||Required||Type||Description||
         |description_en | |String | |
 |description_hin | |String | |
 |description_ur | |String | |
 |do_not_use_it_en | |String | |
 |do_not_use_it_hin | |String | |
 |do_not_use_it_ur | |String | |
 |id | |Long | |
 |status | |String | |
 |use_it_en | |String | |
 |use_it_hin | |String | |
 |use_it_ur | |String | |
        h3. SupplierDriversDTO
        ||Field Name||Required||Type||Description||
         |supplier | |UserItem | |
 |drivers | |TableListOfUserItem | |
        h3. TableListOfNoteDTO
        ||Field Name||Required||Type||Description||
         |list | |array[NoteDTO] | |
 |total | |Long | |
        h3. TableListOfOrderDTO
        ||Field Name||Required||Type||Description||
         |list | |array[OrderDTO] | |
 |total | |Long | |
        h3. TableListOfStatusMessagesDTO
        ||Field Name||Required||Type||Description||
         |list | |array[StatusMessagesDTO] | |
 |total | |Long | |
        h3. TableListOfTransactionDataDTO
        ||Field Name||Required||Type||Description||
         |list | |array[TransactionDataDTO] | |
 |total | |Long | |
        h3. TableListOfUserItem
        ||Field Name||Required||Type||Description||
         |list | |array[UserItem] | |
 |total | |Long | |
        h3. Text_value
        ||Field Name||Required||Type||Description||
         |text | |String | |
 |value | |String | |
        h3. TimeslotDTO
        ||Field Name||Required||Type||Description||
         |available | |Boolean | |
 |custoff_time | |String | |
 |cutoff_time | |String | |
 |description | |String | |
 |end_time | |String | |
 |estimated_delivery_time | |String | |
 |estimated_pickup_time | |String | |
 |id | |Long | |
 |name | |String | |
 |sort_order | |Long | |
 |start_time | |String | |
 |timeslot_availability_id | |Long | |
 |type | |String | |
        h3. TransactionDataDTO
        ||Field Name||Required||Type||Description||
         |cod_charge | |BigDecimal | |
 |completed_date | |Date | |
 |courier_type | |String | |
 |created_date | |Date | |
 |delivery_charge | |BigDecimal | |
 |driver_name | |String | |
 |id | |Integer | |
 |order_code | |String | |
 |order_status | |String | |
 |recipient | |String | |
 |supplier_name | |String | |
 |marketplace_id | |Long | |
        h3. TransactionListDTO
        ||Field Name||Required||Type||Description||
         |currency | |CurrencyDTO | |
 |items | |TableListOfTransactionDataDTO | |
 |total_cod | |BigDecimal | |
 |total_delivery_charge | |BigDecimal | |
 |marketplace_id | |Long | |
 |marketplace_ids | |array[Long] | |
        h3. URI
        ||Field Name||Required||Type||Description||
         |absolute | |Boolean | |
 |authority | |String | |
 |fragment | |String | |
 |host | |String | |
 |opaque | |Boolean | |
 |path | |String | |
 |port | |Integer | |
 |query | |String | |
 |raw_authority | |String | |
 |raw_fragment | |String | |
 |raw_path | |String | |
 |raw_query | |String | |
 |raw_scheme_specific_part | |String | |
 |raw_user_info | |String | |
 |scheme | |String | |
 |scheme_specific_part | |String | |
 |user_info | |String | |
        h3. UserDTO
        ||Field Name||Required||Type||Description||
         |activated | |Boolean | |
 |authorities | |array[String] | |
 |created_date | |String | |
 |email | |String | |
 |first_name | |String | |
 |full_name | |String | |
 |languages | |String | |
 |last_name | |String | |
 |login | |String | |
 |password | |String | |
 |phone | |String | |
 |sanction_cancellation_reason | |String | |
 |sanction_reason | |String | |
 |supplier | |UserItem | |
 |user_id | |Long | |
 |valid_phone | |Boolean | |
 |version | |Integer | |
 |marketplace_id | |Long | |
        h3. UserItem
        ||Field Name||Required||Type||Description||
         |description | |String | |
 |id | |Long | |
 |name | |String | |
 |phone | |String | |
 |photo | |String | |
        h3. UserJWTToken
        ||Field Name||Required||Type||Description||
         |id_token | |String | |
 |user | |UserDTO | |
        h3. UserLocationDTO
        ||Field Name||Required||Type||Description||
         |angle | |Float | |
 |lat | |Double | |
 |lon | |Double | |
        h3. VehicleDTO
        ||Field Name||Required||Type||Description||
         |body_type | |ReferenceDTO | |
 |car_image | |String | |
 |car_registration_card_image | |String | |
 |cargo_capacity | |Double | |
 |color | |ReferenceDTO | |
 |driver | |UserItem | |
 |id | |Long | |
 |make | |ReferenceDTO | |
 |model | |ReferenceDTO | |
 |plate_number | |String | |
 |reg_year | |Integer | |
 |status | |String | |
 |supplier | |UserItem | |
 |type | |String | |
 |vehicle_type | |ReferenceDTO | |
