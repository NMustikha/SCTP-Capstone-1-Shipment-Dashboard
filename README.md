# Capstone on Interactive Dashboards with Excel

## _A Shipment Overview on Delivery Performance_

![Main Dashboard](https://i.gyazo.com/796cb29689f9fc6aa247386d00ec86ed.jpg)
![Secondary Dashboard](https://i.gyazo.com/5300a31ee6e402c1bedfff88f7141be1.jpg)

### [Link to Dataset](https://data.world/usaid/supply-chain-shipment-pricing)

#

### Description of Dataset

The supply chain dataset used in this capstone is from the United States Agency for International Development. It mainly consists of shipment information of Antiretroviral (ARV) and HIV lab commodity itemss to destination countries. This includes the scheduled and actual delivery dates, relevant pricing data of health commodity items and the corresponding freight expenditure to ship the items to their destinations. The dataset has a size of 10,324 rows and is dated from 2006 to 2015.

Some assumptions made on the dataset:

1.	Delivered to Client Date = Actual Delivery Date
2.	Delivered Recorded Date = Order Verification Date
3.	Freight Included in Commodity Cost = Freight Cost is $0 (part of item cost)

### Description of Dashboard

The dashboard mainly focuses on the percentage on time delivery by shipment with the following as secondary information: total orders by shipment, total weight by shipment, total expenditure by shipment, geographical chart of countries, total orders by month and total sum of items by month.

The secondary dashboard is a supplement of the shipments on time delivery by providing more information on each shipment mode’s delivery performance. This is illustrated with the average number of days it takes an item to be delivered by each shipment mode. Separately, another bar chart depicts the maximum and minimum days it takes for an item to be delivered by shipment mode to describe how late (maximum) and how early (minimum) an item is delivered.

### Insights

**_General Observations_**
- Shipment by air charter has the highest on time delivery percentage with truck as the lowest
- Air shipment has the highest number of orders, followed by truck shipment
- Items delivered by truck is the highest
- Most of the expenditure is spent on shipment by air
- Tablet – FDC are significantly shipped more as compared to other commodity items
- Majority of the shipments are delivered to Africa (has one of the highest HIV cases in the world)

**_Analysis_**

**1. Truck shipment is the most cost – effective mode of shipment but its on time delivery is the worst**

Cost-effective whereby it has the highest freight weight and at least half the air shipment cost. Some implications as to why truck shipment could have close to 1000 orders are its convenience to some countries in terms of distance, exclusion of import tax and/or export tax and the inclusion of expenditure in commodity cost

**2. Air shipment could still be the more appropriate shipment mode**

Medications are temperature sensitive and time sensitive. External factors, such as weather and humidity, may affect the efficacy of the medication. Moreover, temperature and humidity can be regulated in cargo planes.

**3. Good to increase inventory stock of tablet and tablet - FDC before Q2 and Q4**

As majority of the commodity items are for HIV treatment, it is not surprising that most of the items shipped are predominantly tablet and tablet – FDC which could be the main type of medication for HIV treatment.

Q1 and Q4 are usually the off peak period (New Year's Day, Christmas) whereby orders may slow down. From past data, usually mid year or closer to December are periods of time where bulk orders are delivered. By preparing surplus before the peak periods, delays could be reduced and on time delivery improves.

### Data Transformation

1. Remove duplicates (no duplicates found in dataset)
2. Formatted custom date (d-mmm-yy) to short date (d/mm/yyyy)
3. Added columns to calculate actual days of delivery and verification
4. Added column to determine if delivery is on time
5. Formatted text under the price columns to currency ($)
6. Added columns to determine rows with numerical freight weight and freight cost
7. Added columns to proper text for selected columns
8. Added columns to group countries into regions and sub regions
9. Remove columns with data dated from 2006 to 2010
10. Remove columns without freight weight and freight cost data

#### [Link to My LinkedIn Profile](https://sg.linkedin.com/in/noor-mustikha-nk)
