# library-primo-ve-normalization

For normalizing MARC data into Primo Normalized Records (PNX) used by the Primo VE service.

[Vendor Documentation](https://knowledge.exlibrisgroup.com/Primo/Product_Documentation/020Primo_VE/Primo_VE_(English)/050Display_Configuration/Configuring_Normalization_Rules_for_Display_and_Local_Fields#Grouping_Conditions)

## Constraints
* Search rule names must include word "Marc" between "Primo VE" and hyphen (-)
* First Rule Name must always be default Rule Name
  * **Display example**: rule "Primo VE - Lds05" 
  * **Search example**:  rule "Primo VE Marc - Lsr01"
* Additional rules begin with same Rule Name as first rule followed by unique text
  * e.g. rule "Primo VE Marc - Lsr01 500"
  * e.g. rule "Primo VE Marc - Lsr01 A"
* Local fields require the first line of text to be the default Rule Name

  ![Example of local field comment](https://github.com/ucsb/library-primo-ve-normalization/blob/master/Img/comment-example.png)
  * All comments must follow first Rule Name
  * Applies to both Search and Display sections

## Front-end result
![Image of Primo VE details service](https://github.com/ucsb/library-primo-ve-normalization/blob/master/Img/details-service-result-example.png)
