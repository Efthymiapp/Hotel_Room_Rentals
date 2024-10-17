# About this Project
It concerns the process of designing and implementing an XML document (**hotel.xml**) that presents a list of available rooms for rent in a hotel, as well as the offers that may be provided for specific rooms at specific time periods. In addition, I also designed a DTD (**hotel.dtd**) that defines the rules that the XML file must conform to in order to ensure the correct structure and validity of the data.

# Description 
- Hotel Information: The Hotel element includes the mandatory properties name and stars, which indicate the name and number of stars of the hotel respectively.
- Rooms List: The Rooms element contains the list of hotel rooms. Each room has a unique id, a name (RoomName), and is described by individual elements such as Capacity, BedTypes, Views, Amenities, and Prices.
 Each room is detailed with the following information:
  * RoomName: The name of the room, with properties such as suite, floor, and wifi.
  * Capacity: The capacity of the room (1-4 people).
  * BedTypes: The number of beds per category (single, double, king size beds, sofa beds).
  * Views: One or more references to the view of the room (eg, sea, mountain).
  * Amenities: A list of room amenities, some of which may be offered for an additional fee.
  * Prices: Room prices per time period (low, medium, high).
- List of Offers: The Offers element contains a list of offers, which can be empty. Each offer contains the following information:
  * roomId: Reference to the rooms to which the offer applies.
  * price: The price of the offer.
  * Name: Optional name for the offer.
  * Period: The period during which the offer is valid, with mandatory from and to properties.
