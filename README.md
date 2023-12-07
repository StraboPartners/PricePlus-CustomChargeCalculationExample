
# Strabo Price Plus

## Example custom charge calculation methods

This repo contains examples of how a custom charge calculation method can be implemented

The `ExampleSalesHeaderMethod` class contains a real implementation for sales header charges. 
The `ExampleAllTypesMethod` shows the structure for implementation support for all charge types. 

## Details

Custom charge methods are implemented by creating a class that implements the appropriate interface depending on the type of charge to be supported. 

- `SPRISalesHeaderChargeCalculationMethod` for sales header charges
- `SPRISalesLineChargeCalculationMethod` for sales line charges
- `SPRISalesLineChargeCalculationMethod` for purchase header charges
- `SPRIPurchaseLineChargeCalculationMethod` for purchase line charges

When a class implements the interface, it will show up in the UI dropdown for users to select when configuring a charge with a calculation method.