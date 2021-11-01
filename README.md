# StarbucksCapstone
Udacity - Starbucks Capstone Project

# Project Introduction:  
  
**_from project requirements_**  
This data set contains simulated data that mimics customer behavior on the Starbucks rewards mobile app. Once every few days, Starbucks sends out an offer to users of the mobile app. An offer can be merely an advertisement for a drink or an actual offer such as a discount or BOGO (buy one get one free). Some users might not receive any offer during certain weeks.

Not all users receive the same offer, and that is the challenge to solve with this data set.

Your task is to combine transaction, demographic and offer data to determine which demographic groups respond best to which offer type. This data set is a simplified version of the real Starbucks app because the underlying simulator only has one product whereas Starbucks actually sells dozens of products.

Every offer has a validity period before the offer expires. As an example, a BOGO offer might be valid for only 5 days. You'll see in the data set that informational offers have a validity period even though these ads are merely providing information about a product; for example, if an informational offer has 7 days of validity, you can assume the customer is feeling the influence of the offer for 7 days after receiving the advertisement.

You'll be given transactional data showing user purchases made on the app including the timestamp of purchase and the amount of money spent on a purchase. This transactional data also has a record for each offer that a user receives as well as a record for when a user actually views the offer. There are also records for when a user completes an offer.

Keep in mind as well that someone using the app might make a purchase through the app without having received an offer or seen an offer.  

**#Libraries used**  
pandas  
numpy  
math  
datetime  
json  
matplotlib  
seaborn (v 0.11.2) 

execute following lines to get the latest version  
`import sys`  
`!{sys.executable} -m pip install seaborn==0.11.2`  

# Data files
Data files are contained in the data.zip file. Unzip and copy these in the data folder

**from project description**
The data is contained in three files:

portfolio.json - containing offer ids and meta data about each offer (duration, type, etc.)
profile.json - demographic data for each customer
transcript.json - records for transactions, offers received, offers viewed, and offers completed


# Conclusion  
------------------------------------------
Evaluating the Female Demography
------------------------------------------

**Female - send bogo offer to the 27 out of 84 age group**   
 [ 18  19  21  24  25  26  27  29  32  33  34  36  39  41  44  45  49  52  53  55  83  85  91  93  94  98 100]   
 
**Female - send discount offer to the 57 out of 84 age group** 
 [ 20  22  23  28  30  31  35  37  38  40  42  43  46  47  48  50  51  54  56  57  58  59  60  61  62  63  64  65  66  67  68  69  70  71  72  73
   74  75  76  77  78  79  80  81  82  84  86  87  88  89  90  92  95  96  97  99 101] 
 
**Female - dont send informational offer to the 55 out of 84 age group**   
 [ 21  24  25  26  31  33  36  40  41  43  44  45  47  48  49  50  51  52  53  54  57  60  61  63  64  65  66  67  68  69  71  72  73  74  76  78
  79  80  81  83  84  85  86  87  88  89  90  91  92  93  94  96  98  99 100] 
 
**Female - send informational offer  to the 29 out of 84 age group **  
 [ 18  19  20  22  23  27  28  29  30  32  34  35  37  38  39  42  46  55  56  58  59  62  70  75  77  82  95  97 101] 
 
------------------------------------------
Evaluating the Male Demography
------------------------------------------

**Male - send bogo offer to the 28 out of 83 age group**   
 [21 23 34 36 37 39 41 42 44 46 48 52 53 54 59 61 62 73 75 80 83 86 88 89
 92 95 97 99] 
 
**Male - send discount offer to the 55 out of 83 age group**   
 [ 18  19  20  22  24  25  26  27  28  29  30  31  32  33  35  38  40  43
  45  47  49  50  51  55  56  57  58  60  63  64  65  66  67  68  69  70
  71  72  74  76  77  78  79  81  82  84  85  87  90  91  93  94  96  98
 100] 
 
**Male - dont send informational offer to the 65 out of 83 age group**   
 [ 18  20  23  24  25  28  29  31  32  34  35  36  37  38  39  41  42  43
  44  45  46  47  48  49  50  51  52  53  55  56  59  60  61  62  63  64
  65  66  67  68  69  70  71  72  73  74  75  76  79  80  81  82  84  86
  88  89  90  91  93  94  95  96  97  99 100] 
 
**Male - send informational offer  to the 18 out of 83 age group**   
 [19 21 22 26 27 30 33 40 54 57 58 77 78 83 85 87 92 98] 
 
------------------------------------------
Evaluating the Other Demography
------------------------------------------

**Other - send bogo offer to the 30 out of 66 age group**   
 [22 24 25 26 28 35 36 38 39 40 42 43 44 45 47 50 53 54 55 56 67 69 70 71
 73 75 77 81 82 85] 
 
**Other - send discount offer to the 31 out of 66 age group**  
 [20 21 30 31 32 33 34 37 41 46 48 49 51 52 57 58 59 60 61 62 63 64 66 68
 74 76 79 84 89 90 92] 
 
**Other - send any, bogo or discount offer to the 5 out of 66 age group**  
 [ 29  65  72  80 100] 
 
**Other - dont send informational offer to the 47 out of 66 age group**  
 [ 20  21  24  25  26  29  30  32  33  34  35  36  37  38  39  40  42  44
  45  47  48  50  51  52  53  54  56  57  60  63  64  65  66  69  71  72
  74  75  79  80  81  82  85  89  90  92 100] 
 
**Other - send informational offer  to the 19 out of 66 age group**   
 [22 28 31 41 43 46 49 55 58 59 61 62 67 68 70 73 76 77 84] 
