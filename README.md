# FIWARE Data Models

![](https://nexus.lab.fiware.org/static/badges/statuses/deprecated.svg)
[![License: MIT](https://img.shields.io/github/license/FIWARE/data-models.svg)](https://opensource.org/licenses/MIT)
<br/>

> This repository is now archived and subsequent works will be carried out in
> [Smart data models](https://github.com/smart-data-models) repositories.

This repository contained:

-   [JSON Schemas and documentation](./specs/README.md) on harmonized datamodels
    for different Smart Domains, particularly **Smart Cities** and **Smart
    Agrifood**.
-   code that allows to expose different harmonized datasets useful for
    different applications. Such datasets are currently exposed through the
    [FIWARE NGSI version 2](http://fiware.github.io/specifications/ngsiv2/stable)
    and/or
    [NGSI-LD](https://www.etsi.org/deliver/etsi_gs/CIM/001_099/009/01.01.01_60/gs_CIM009v010101p.pdf)
    APIs (query).

This work was aligned with the results of the
[GSMA IoT Big Data](https://www.gsma.com/iot/iot-big-data/) Project. Such
project is working on the harmonization of APIs and data models for fueling IoT
and Big Data Ecosystems. In fact the FIWARE data models are a superset of the
[GSMA Data Models](https://github.com/GSMADeveloper/NGSI-LD-Entities).

Some of the Data Models in this Repository have been adopted by a joint
initiative between TM Forum and FIWARE Foundation. For more info please check
[https://github.com/smart-data-models/dataModels](https://github.com/smart-data-models/dataModels)

| :books: [Documentation](https://fiware-datamodels.rtfd.io) |
| ---------------------------------------------------------- |

## Data Models adoption

To support the adoption, we created a short [guideline](specs/howto.md) for the
usage of data models. If you are using **NGSI-LD**, you should also check the
[NGSI-LD HowTo](./specs/ngsi-ld_howto.md) and the
[NGSI-LD FAQ](./specs/ngsi-ld_faq.md).

## JSON Schemas

A [JSON Schema](http://json-schema.org/) was provided for every harmonized data
model. There are different online JSON Schema Validators, for instance:
[http://jsonschemalint.com/](http://jsonschemalint.com/). For the development of
these schemas the
[AJV JSON Schema Validator](https://github.com/epoberezkin/ajv) is being used.
For using it just install it through npm:

```console
npm install ajv
npm install ajv-cli
```

A `validate.sh` script is provided for convenience.

**Note**: JSON Schemas capture the name and data type of each Entity Attribute.
For instance, this means that to test JSON schema examples with a
[FIWARE NGSI version 2](http://fiware.github.io/specifications/ngsiv2/stable) or
[NGSI-LD](https://www.etsi.org/deliver/etsi_gs/CIM/001_099/009/01.01.01_60/gs_CIM009v010101p.pdf)
API implementation, you need to use the `keyValues` mode (`options=keyValues`).

## Related Projects

See:

-   [https://gitlab.com/synchronicity-iot/synchronicity-data-models](https://gitlab.com/synchronicity-iot/synchronicity-data-models)
-   [schema.org](https://schema.org)
-   [https://github.com/GSMADeveloper/NGSI-LD-Entities](https://github.com/GSMADeveloper/NGSI-LD-Entities)
-   [https://forge.etsi.org/gitlab/NGSI-LD/NGSI-LD](https://forge.etsi.org/gitlab/NGSI-LD/NGSI-LD)

---

## License

### Code

[MIT](LICENSE) © 2019-2021 FIWARE Foundation e.V.

[![License: MIT](https://img.shields.io/github/license/FIWARE/data-models.svg)](https://opensource.org/licenses/MIT)

All the code in this repository is licensed under the MIT License. However each
original data source may have a different license. So before using harmonized
data please check carefully each data license.

### Models

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

All the data models documented here are offered under a
[Creative Commons by Attribution 4.0](https://creativecommons.org/licenses/by/4.0/)
License.
