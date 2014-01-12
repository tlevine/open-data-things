Benn has trouble handling uploads of CSVs
(without strongly typed columns) to modeanalytics

I could model column typing with open data.




The brainstorm with Carter:


    HumanTemp \/ AllCapsAddy \/  (A /\ B)
   
    ->>> [FormatPredicts]
   
   
    type Column = Stream (RowId,Text)  -- Stream left updefine dfor now :)
   
    data FormatPredicate  =  FPred  (Text -> Infos)
   
    data Infos =  forall a . (Show a)=> MkInfo Bool a
   
   
    runPredictes ::   [FormatPredicates]-> Column -> PredicateReport


My turn:



    Each row is a column in a dataset

    datasetId,columnName,       min,  max, has.point, has.digits, sd,
    matches.whatever.regex
    1,        id,                           .7324
    1,        name,
    1,        address,
    1,        blood.pressure,

