import sqlite3

def connect(dbname):

  conn = sqlite3.connect (dbname))

  conn.execute("CREATE TABLE IF NOT EXISTS OYO HOTELS (NAME TEXT, ADDRESS TEXT, PRICE INT, AMENITIES TEXT, RATING TEXT)")

print("Table created successfully!")

conn.close()

def insert_into_table('dbname, values):

conn = sqlite3.connect(dbname)

print("Inserted into table: " + str(values))

insert_sql = "INSERT INTO OYO HOTELS (NAME, ADDRESS, PRICE, AMENITIES, RATING) VALUES (?, ?, ?, ?, ?)"

conn.execute(insert_sql, values)

conn.commit()

conn.close()

def get_hotel_info(dbname):

conn = sqlite3.connect(dbname)
for hotel in all hotels:

hotel dict = 0

hotel_dict["name"]= hotel.find("h3", "class": "listingHotelDescription hotelName"}).text hotel_dict["address"]= hotel.find("span", ("itemprop": "streetAddress"}).text hotel_dict ["price"]= hotel.find("span", ("class": "ListingPrice_finalPrice")).text

#try except

try:

hotel_dict["rating"] = hotel.find("span", "class": "hotelRating_ratingSummary")).text. except AttributeError:

pass

parent_amenities element = hotel.find("div". ("class": "amenitywrapper">)

amenities list = []

for amenity in parent_amenities element.find_all("div", ("class": "amenityWrapper_amenity"}}: amenities List.append(amenity.find("span", {"class": "d-body-sm")).text.strip())

hotel_dict["amenities"]=, .join(amenities_list[:-1])

scraped_info_list.append(hotel_dict)

connect.insert_into_tablelargs.dbname, tuple(hotel_dict.values()))

dataFrame =pandas.DataFrame(scraped_info_list)

 print("Creating csv file...")

dataFrame.to_csv ("Oyo.csv".)

connect.get_hotel_infolargs.dbname)
