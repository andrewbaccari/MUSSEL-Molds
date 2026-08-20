# MUSSEL-Molds
This repository hosts the SolidWorks files for deep-sea pressure-rated cable splicing.

**Required Items**

**Software & Equipment**
- SolidWorks 2025 (or later)
- PreForm (Formlabs slicing software)
- Resin printer
- Pressure chamber
- Calipers
- High-grit sandpaper

**Materials & Hardware**
- 3M Scotchcast 2131, 7.5 oz
- Formlabs Clear V4.1 or Clear V5 resin
- 6x 1/4" hex nuts
- 6x 1/4-20, 0.75" screws


**1. SolidWorks Setup**
    Modify the mold's hole diameters to fit your cables.
- Using calipers, measure the outer diameter of each cable you want to pot together. Cable diameter must not exceed 11.4 mm.
- Open SolidWorks and open TopMold.SLDPRT.
- In the left-hand tree, right-click Equations and select Manage Equations.
- Under the Value / Equation column, enter the measured diameters for the Left and Right cable.
- Open BottomMold.SLDPRT and repeat the past two steps.
- Open MUSSELAssem.SLDASM and confirm that both cable holes appear circular.

**2. Printing**
    This step is only needed once, unless you're changing cable sizes.
- FDM or SLA print Foot.SLDPRT (only needs to be done once).
- Open PreForm and upload TopMold.SLDPRT and BottomMold.SLDPRT.
- Orient both parts with their flat sections facing up. This prevents supports from generating on that face and keeps it as flat as possible for sealing the faces together.
- Add supports and start the print.

**3. Post-Printing**
- Remove the parts from the build plate.
- Wash them in isopropyl alcohol.
- Cure according to resin type:
    - Clear V4.1: 15 min at 60 °C
    - Clear V5: 5 min, no heat
    - For other resins, check Formlabs's Form Cure V1 time/temperature guide.
- Remove all supports.

**4. Lapping**
    Ideally a one-time step, unless the mold faces get damaged.
    The flat mating faces of the TopMold and BottomMold must be perfectly flat to form a seal.
- Lay a sheet of high-grit sandpaper on a flat, rigid surface.
- Lap both mold halves flat against it.
- Work carefully and check often — over-sanding will remove too much material and prevent the mold from sealing around the cable.

**5. Mold Release**
    In a well-ventilated area (ideally outdoors), apply mold release to the internal cavity of both mold halves.
- Err on the side of applying more as it eases disassembly later and produces a cleaner final part.

**6. Assembly**
- Slide the Foot onto the BottomMold.
- Place the cable(s) into the BottomMold and set the TopMold on top.
- Confirm the cable runs straight through the mold and isn't touching the inner walls.
- Insert the six hex nuts into the BottomMold and thread the screws through the TopMold in an X pattern to distribute clamping pressure evenly.

**7. Scotchcasting**
    A 7.5 oz bag comfortably fills two molds — consider assembling two MUSSEL molds at once if you have the parts on hand.
- Follow the mixing instructions on the 3M Scotchcast 2131 bag, with one change: mix for 90 seconds instead of the recommended 30, making sure to work resin out of every corner of the bag.
    - Do not undermix. An incomplete cure will compromise the seal, and the affected section of cable will need to be cut out, resoldered, and repotted from scratch.
- Snip a small corner off the bag and slowly pour the resin into the TopMold's fill hole until it reaches near the top.

**8. Pressure Potting**
    Compresses air bubbles trapped in the Scotchcast for a stronger, more reliable seal.
- Place the assembled MUSSEL mold into the pressure pot with the TopMold's fill hole facing up.
- Close and secure the pressure pot lid.
- Bring the chamber to 45 PSI and hold for 8+ hours. (Starting this at the end of the day so it runs overnight works well.)

**9. Disassembly**
    Do not use a metal scraper directly on the mold. It will scratch the flat sealing surfaces, requiring you to relap the mold — and risking sanding it too thin to reseal.
- Peel the two mold halves apart slightly and slide a plastic scraper into the gap.
- Slide a second plastic scraper in under the first.
- Wedge a metal scraper between the two plastic scrapers and twist to help separate the halves.
- If the BottomMold comes away still attached to the TopMold, use a handled hex driver through the TopMold's fill hole to carefully push the cured Scotchcast resin free.

Done. Your cable splice is potted, pressure-cured, and depth-rated.
