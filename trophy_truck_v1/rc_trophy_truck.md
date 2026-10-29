# 3D Printed RC Trophy Truck

*A 1:10 scale, trophy-truck-inspired RC car with a 3D printed body.*

This write-up covers the design and build of my 1:10 scale RC truck, which has a 3D printed body and premade electronic components. My goals were to make a functional, durable and stylised truck, to find out which parts could be 3D printed, and to practise iterative design and CAD in preparation for future 3D printed projects. There was no fixed budget, since I ordered parts as I needed them and spent money on unplanned R&D. The total was around \$[cost], including duplicates and unused parts. The project taught me some important lessons about design, building and RC control systems.

<p align="center">
  <a href="RC_Car_V1/front_corner_posed.jpg"><img src="RC_Car_V1/front_corner_posed.jpg" width="500" alt="The finished truck"></a><br>
  <em>The finished truck.</em>
</p>

**At a glance**

- **Type:** 1:10 fully custom electric trophy truck
- **Timeline:** 6 months, roughly 100 hours of work
- **Budget:** No fixed budget, about \$[cost] in total including duplicates and unused parts
- **Result:** A truck capable of gravel, dirt and jumps
- **Skills:** CAD, 3D printing, soldering, system integration, iterative design

---

## Why I built it

After designing and building my [foam RC plane](RC_Plane.md), I bought a 3D printer. I was eager to start a project with it, and a custom RC car was a natural choice, since cars are the type of RC vehicle I have the most experience with. This time I wanted a truck that could jump, and I took inspiration from trophy truck suspension: a 4-link rear and double wishbone front.

Early decisions that shaped the design:

- **Suspension:** The project was built around long-travel trophy truck suspension, so the drivetrain, power system, steering, body and scale were all decided from there.
- **Scale:** I chose 1:10 as the middle ground. It's large enough for strong 3D printed parts and for suspension to matter, and small enough that the motor and other bought parts wouldn't be too expensive. I also owned a 1:10 short course truck to use as a reference.
- **Motor:** I considered nitro (liquid fuel), brushed electric and brushless electric. I chose brushless electric for enough power, durability and simplicity.

---

## Design and dimensions

The design was inspired by Baja trophy trucks, where a solid 4-link rear axle and independent front suspension give great stability and travel. My custom design had to house a drive motor, steering servo, gearing and driveshaft, rear axle, front and rear wheels, and the suspension.

<p align="center">
  <a href="RC_Car_V1/Example_Truck.jpg"><img src="RC_Car_V1/Example_Truck.jpg" width="600" alt="Baja trophy truck"></a><br>
  <em>Design inspiration: a Baja trophy truck.</em>
</p>

I calculated the scaled body length and width from standard trophy truck dimensions, along with a rough body and shell shape. I designed from the front to the back. The front was the most complex section and needed the most precision, so the body and rear followed from it.

<p align="center">
  <a href="RC_Car_V1/design_sketches_scale.jpg"><img src="RC_Car_V1/design_sketches_scale.jpg" width="600" alt="Design sketches"></a><br>
  <em>Sketches exploring the shape of the truck.</em>
</p>

- **Scale / type:** 1:10
- **Wheelbase / track width:** [ ]
- **Drivetrain:** Rear-wheel drive. It started as 4WD, but 2WD was simpler and more durable.
- **Suspension:** Independent double wishbone at the front, long-travel solid axle with 4-link at the rear
- **Tyres:** [ ]
- **Weight:** [ ] g including battery

---

## Stage 1: The front

The front needed to house the two independent spring and shock units, the shock tower, wheel hubs and joints, and the steering arms and links. That meant it had a lot of moving parts, all of which had to reach their extremes without interfering with each other. It also had to be strong, since it takes the brunt of impacts and collisions.

<p align="center">
  <a href="RC_Car_V1/front.jpg"><img src="RC_Car_V1/front.jpg" width="500" alt="Front chassis and suspension"></a><br>
  <em>The front section of the truck, face on.</em>
</p>

**Problem: the parts were hard to design to spec while staying strong.** At this small scale, with so many moving parts, the first system I simplified was the drivetrain, changing from 4WD to rear-wheel drive. This greatly simplified the wheel hubs, and I had also run into gearing issues while planning the drivetrain.

<p align="center">
  <a href="RC_Car_V1/all2.jpg"><img src="RC_Car_V1/all2.jpg" width="500" alt="Front component iterations"></a><br>
  <em>Several iterations of mostly front-end parts laid out together, from first prototypes (grey PLA, cheaper but less durable) to final versions (white PETG, more durable but more expensive).</em>
</p>

---

## Stage 2: Body and rear

[What the rear needed to do, how you designed the 4-link rear suspension and the main body, and what went wrong.]

<p align="center">
  <a href="RC_Car_V1/rear_close.jpg"><img src="RC_Car_V1/rear_close.jpg" width="500" alt="Rear axle and 4-link suspension"></a><br>
  <em>[Caption.]</em>
</p>

---

## Motor, electronics and radio

[How you chose and installed the electronics, how long setup took, and anything you found hard that would help the next builder.]

- **Motor:** [model, kV or turns]
- **ESC:** [amp rating]
- **Battery:** [cells, mAh, C rating]
- **Radio:** [transmitter and receiver]
- **Servo:** [type]

---

## Final touches

[Body finishing, set-up and tuning, and final checks.]

---

## Cost

[One or two sentences: you had no fixed budget, you ordered parts as you went, the total was \$[cost], and how much of that went on duplicates, unused parts and reprints.]

---

## Results

[Test conditions: location, surface, weather, battery used.]

- **Performance:** [top speed, run time, acceleration, with numbers if you have them]
- **Handling:** [how it drove, and what limited it]
- **Durability:** [crashes, rollovers, repairs, how many runs]

[2 to 3 sentences on how the results compare with your goals, and what they say about the design.]

[Add your driving video here: drag `driving_video.mp4` into the GitHub editor, leave a blank line after the link, and put the caption in a separate paragraph.]

---

## What I'd do differently

- Design or buy stronger joints that allow more movement and more degrees of freedom
- Spend more time integrating the delicate moving parts, such as the steering and driveshaft, so they have enough clearance and aren't restricted
- Design connection points that are easier to access, quicker to use and stronger
- Design more simply, with more flexibility for changes later
- Try 3D printing the axles and drivetrain, or build them from base materials (such as metal rods) combined with 3D printing, cutting and shaping, instead of buying complete components

**Biggest lesson:** for iterative design, parts need to be smaller and easier to print, connect, remove and replace, to cut down on wasted time, filament and broken components. One of my largest problems was that I had designed myself into a corner. I made large components that only worked in specific ways, then designed other components to depend on them. That limited my flexibility, and I spent a lot of effort on quick fixes to fundamental problems. Examples:

- Redesigning the rear linkages to improve joint flexibility and strength, instead of switching to a separate joint mechanism or moving the joint points
- Redesigning the main body section to fit the motor mount, bearing and driveshaft mount. This was poorly designed from the start, since tensioned belt systems work poorly in small, flexible and relatively weak printed parts.
- Reprinting and reattaching the front body section after it broke from stress concentrated at poorly designed joints
- Editing and reprinting body and steering parts because the front wheels rubbed and stuck against the body in sharp turns, when redesigning the steering or adjusting the front body to suit the wheels would have fixed it

---

## Gallery

<p align="center">
  <img src="RC_Car_V1/front_corner_posed.jpg" width="48%" alt="Front corner view">
  <img src="RC_Car_V1/front_corner_posed2.jpg" width="48%" alt="Front corner view from another angle"><br>
  <em>Front corner views of the finished truck.</em>
</p>

<p align="center">
  <img src="RC_Car_V1/side_posed.jpg" width="48%" alt="Side view">
  <img src="RC_Car_V1/top.jpg" width="48%" alt="Top view"><br>
  <em>Side and top views showing the layout.</em>
</p>

<p align="center">
  <img src="RC_Car_V1/front_action.jpg" width="48%" alt="Front suspension in action">
  <img src="RC_Car_V1/front_action2.jpg" width="48%" alt="Front suspension in action, second angle"><br>
  <em>The independent front suspension flexing over an obstacle.</em>
</p>

<p align="center">
  <img src="RC_Car_V1/rear_action.jpg" width="48%" alt="Rear suspension in action">
  <img src="RC_Car_V1/rear_action2.jpg" width="48%" alt="Rear suspension in action, second angle"><br>
  <em>The 4-link rear suspension over the same obstacle.</em>
</p>

<p align="center">
  <img src="RC_Car_V1/close1.jpg" width="48%" alt="Close-up of the electronics">
  <img src="RC_Car_V1/rear2.jpg" width="48%" alt="Top-down view of the rear">
  <br>
  <em>A close-up of the electronics, and a top-down view of the rear axle and drivetrain.</em>
</p>
