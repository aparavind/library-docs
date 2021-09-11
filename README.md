# Object Management System
We have seen a number of things are unmanaged in a house. For eg. books are scattered everywhere in the house. and we are not even sure what books are there and what are not there.

This Application tries to mantain accountability. so that we are able to search and retain them. This

This application does no magic . we need to feed them with proper information in order to get proper results.

## Componants
1.  Client
    1.  Android
    1.   Web-html (Angular)
1.  Server
    1.  C++
1.  Database(s)
    1. MySQL
    1. Redis
1.  Intercomponant communication
    1.  GRPC Protocol

## Architecture
Baisically it will have the following modules.
1.  STORAGE
    1.  __ACCOUNT__: just in case we get to multi account product
    1.  __HOUSE__ : Books / utensils or anything for that matter is primarily present in a house. one account may have multiple houses.
    1.  __RACK__ : this is the rack where induvidual books are kept . however it can also be a kitchen shelf for utensils in short any place to keep things
    1.  __SHELF__ : this is the induvidual unnit that will keep a max of upto 8 items. (More than 8 you need to split the shelf)
    1.  __ITEM__ : the primary focus or the recorded thing . it will be placed in a shelf.

    so basically an item is kept in a shelf which is kept in a rack which is kept in a house and which belongs to an account.
