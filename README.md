# Petstore

<!-- Start SDK Installation -->
## SDK Installation

### Gradle

```groovy
implementation 'speakit.Petstore:Petstore:1.0.0'
```
<!-- End SDK Installation -->

## SDK Example Usage
<!-- Start SDK Example Usage -->
```java
package hello.world;

import speakit.Petstore.Petstore;
import speakit.Petstore.models.operations.CreatePetsResponse;

public class Application {
    public static void main(String[] args) {
        try {
            Petstore sdk = Petstore.builder()
                .build();

            CreatePetsResponse res = sdk.pets.createPets();

            if (res.statusCode == 200) {
                // handle response
            }
        } catch (Exception e) {
            // handle exception
        }
    }
}
```
<!-- End SDK Example Usage -->

<!-- Start SDK Available Operations -->
## Available Resources and Operations


### [pets](docs/pets/README.md)

* [createPets](docs/pets/README.md#createpets) - Create a pet
* [listPets](docs/pets/README.md#listpets) - List all pets
* [showPetById](docs/pets/README.md#showpetbyid) - Info for a specific pet
<!-- End SDK Available Operations -->

### Maturity

This SDK is in beta, and there may be breaking changes between versions without a major version update. Therefore, we recommend pinning usage 
to a specific package version. This way, you can install the same version each time without breaking changes unless you are intentionally 
looking for the latest version.

### Contributions

While we value open-source contributions to this SDK, this library is generated programmatically. 
Feel free to open a PR or a Github issue as a proof of concept and we'll do our best to include it in a future release !

### SDK Created by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-speakeasy/client-sdks)
