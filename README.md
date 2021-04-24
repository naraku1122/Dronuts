**Context**

    Two of your close friends run a successful artisanal donut shop in Lawrenceville, PA. Looking for ways to expand their business, they reach out to you, knowing that you will apply your skills for startup engineering to the problem.

**Background: Donuts**
    Donuts are America's favorite pastry, topping $15bn1 in sales annually. However, two key factors have limited their market saturation:

Short shelf-life
    Unlike other pastries (like cookies or muffins), donuts retain optimal texture for only one to two days after baking. This means they must be sold quickly after baking and consumed rapidly, making efficient distribution essential.

Poor afternoon sales
    Most people buy donuts out of convenience while purchasing their morning coffee. Rival donut company Dunkin' Donuts reported to shareholders that approximately 70% of their sales occur before 11am.2 This likely indicates an untapped market of individuals who are interested in purchasing donuts, but find it too inconvienient after their morning stop.

**Background: Drones**
    A reclusive (and entirely fictional) genius has finally developed a safe and cost-effective lithium-air3 battery! This technology enables the development of lightweight unmanned aerial vehicles (UAVs), better known as drones. These new batteries improve the flight time of small drones (the size of the Iris Pixhawk+,4 say) by an order of magnitude (from 16-20 minutes to 1-2 hours).

    Inspired by Elon Musk's decision to open-source Tesla's patents, 5, the inventory decided to do the same with his battery. This led to the commoditization of drone-based mobility, which has redefined the way we use drones in a number of ways:

    DroneTech, a major player in the UAV market, has created a highly advanced drone mobility solution; enabling you to purchase off-the-shelf drones, and send them to perform deliveries using a REST API.
    Capitalizing on this, Amazon Prime Air, a drone delivery service for retail items, has seen mainstream use. Most consumers have designated drone delivery points at their home, making delivery failures unlikely.
    The widespread adoption of drone technologies has led to modification of FAA regulations on drone usage, allowing platforms like DroneTech's to opaquely negotiate airspace access with FAA servers.
    This is exciting; these developments alleviate most of the fundamental barriers to home delivery of a cheap good via drone.

**Your Idea**

    You have a brainflash: software built atop the DroneTech API, coupled with a small fleet of the new drones, could help you capitalize on the vast untapped afternoon donut market! Your donut-making friends are intrigued, and think drone-based donut delivery could work. They're not very tech-savvy, and they have their hands full with the existing business, so they'd rather serve as your first partner/supplier than as co-founders. However, they have a couple of other friends at CMU, to whom they introduce you. With those classmates, you officially found Dronuts, a startup company which delivers fresh donuts via drone. You pool your resources and buy an initial fleet of 6 drones.

**Your Product**

    Your basic idea is to build a cloud-backed web application,6 with which several types of users will interact, approximately as follows:

     - A donut-buying customer will use the app to select donuts from a menu of items offered by the donut shop.
     - The app will redirect customers to an external payment service, CommerceFriend, to enter payment details for their items.
     - The app will identify a suitable drone to perform the delivery based on availability and battery life. Various factors may influence battery life, including distance,        weight of the package, and weather/wind. Fortunately, DroneTech's API includes a sophisticated algorithm for managing battery capacity, allowing the drone to                  automatically return to the shop if the battery level is critical.
     - The app will relay the order to the donut shop in Lawrenceville, and will instruct employees which drone items are to be loaded into. Once loaded, the app should send        the drone out for delivery.
     - The customer will be able to track the progress of their delivery in real-time using the app, so they know when to retrieve the items from the drone. (For the purposes        of the course, you don't need to worry about the actual physical drone hardware beyond the software considerations surrounding battery life.)

    This initial outline is deliberately open-ended, as we intend for you to apply and practice the skills you learn in this class in a realistic startup context. Over the course of the first half of the semester (eight weeks), you will work with your classmates to design, implement and analyze the software for this (hyopthetical) new startup.

**End game?**

You envision a number of ways this idea might make you fantastically wealthy. Maybe you and your friends will build a country-spanning artisinal delivery donut shop empire. Maybe Amazon Go will take an interest, and acquire you for a fantastic sum. Maybe Dunkin' Donuts will agree to license your SaaS platform, again for a fantastic sum. The sky's the limit! You just need to get the whole thing off the ground...

**Citations and Footnotes**

1: IBIS World 2017.
2: Dunkin' Donuts U.S. Marketing 2015.
3: Lithium-air batteries have been a theoretical possibility and the subject of research for decades. Wikipedia has more.
4: The IRIS quadcopter.
5: "All Our Patents are Belong to You", Tesla blog, 06/12/2014
6: The course staff acknowledges that a mobile app probably does make more sense in this context; we are stipulating a web application for pedagogical purposes.
