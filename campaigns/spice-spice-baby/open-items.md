# Spice Spice Baby, open items

Internal. Do not send to press. Last reviewed 2026-09-10 against the Framer CMS
(`Menu Items` collection, category "Limited Time Only"), the kitchen recipe card
for the pancakes, and the live page at https://www.wildeggs.com/menu/fall-lto

The CMS is the source of truth for the fact sheet. All seven LTO items carry a
complete record: title, price, ingredient-level description, per-item allergens
and a menu image. Cross-checked against the seven cards rendering on the live
page, and they match.

## Fix before launch

1. **The Pumpkin Pie Pancakes allergen list omits tree nuts.** The recipe card
   puts 2 oz of candied pecans on every plate. The CMS allergen field reads
   `egg | milk | soy | wheat` and the nutrition block published on the site says
   "Egg, Milk/Dairy, Soy, Wheat/Gluten." Tree nuts have to be added to both. This
   is a guest-safety fix, not a copy preference, and it is live on the site now.

2. **Confirm the gluten-free build and its allergens.** If the gluten-free stack
   takes the same caramel, pecans, whipped cream and dusting, it also contains
   tree nuts, and its CMS allergen field currently reads `egg | milk` only. We
   have no recipe card for it. Its description still says "ask your server for
   the full build," which is the one item on the sheet a reporter cannot get a
   straight answer about.

3. **Update the CMS pancake description to the real build.** The record still
   describes the batter only and says "stacked tall." It is a two-cake plate
   spread to 8" on a 12" round, finished with salted vanilla caramel, candied
   pecans, whipped cream, powdered sugar and cinnamon. New copy is in the fact
   sheet; the card is in `recipes/pumpkin-pie-pancakes.md`.

## The landing page under-reports what we already have

4. **Only two of seven items show a description on `/menu/fall-lto`.** The Hot
   Honey Chicken Sandwich and the Pumpkin Pie Pancakes have body copy in the page
   layout. The Sunrise Tostadas, Spicy Mary, Caramel Apple Spice Mimosa, The Wild
   Pumpkin and the gluten-free stack render as image cards with a badge and
   nothing else, and the tostada and mimosa prices appear nowhere on the page.
   All of that content exists in the CMS. This is a page-binding gap, not a copy
   gap, and worth fixing, since it is why a reporter had to ask us for the list.

5. **The FAQ names the gluten-free item wrong.** The FAQ block says "GF Pumpkin
   Patch Cakes." The CMS title is "Gluten-free Pumpkin Pie Pancakes." Pumpkin
   Patch Cakes is the Rise & Fall item name.

6. **Two variants of the hero paragraph are in the markup.** One ends "spice up
   your fall," the other ends "turn up the spice." There are also fragmented headline states
   ("Sweet and heat", "heat has", "have entered"). Confirm these are intended
   animation states and not stray drafts.

7. **Alt-text errors.** The full-plate sandwich image
   (`zVHkDlCvJ3VOdfgmbexiVmPPPYA.jpeg`) carries the alt text "Enjoying Bottomless
   Mimosas at Wild Eggs" in one placement. The gluten-free pancake image has the
   typo "GF Pumpkin Panakes." The pumpkin pancake image still carries a leftover
   template alt, "Abstract shadows of a tree cast on a light surface."

## CMS data hygiene

8. **Spicy Mary "Price - Large" is `12.99`, missing the dollar sign**, while
   "Price - Medium" is `$12.99`. Every other item formats both fields the same
   way. Fix before anything renders off the Large field.

9. **Caramel Apple Spice Mimosa has an empty "Price - Large".** Harmless today,
   but the other six items populate it, so it will read as a gap if a component
   starts using that field.

10. **Nutrition is a placeholder on six of seven items**: "Full nutrition
    information for this seasonal item is coming soon." The gluten-free stack says
    "Ask your server" instead. If a reporter asks for calories we cannot answer.

## Copy decisions worth knowing

11. **The sandwich build changed from the tasting notes and the CMS is right.**
    Earlier copy described chicken "marinated in buttermilk and Frank's" with hot
    honey applied on top and the chipotle slaw as a cooling side. The CMS build is
    hand-breaded chicken *tossed* in house-made hot honey, with the chipotle slaw
    as a base *under* the waffle and also served on the side. The fact sheet
    follows the CMS.

12. **Sub-recipe detail is deliberately not in the fact sheet.** The campaign copy
    doc breaks the hot honey down to Frank's RedHot, clover honey and real butter.
    The CMS says "house-made hot honey sauce." Naming suppliers to a trade reporter
    is a call for Elle, so the sheet stays at the CMS level. The detail is there if
    we want to offer it. Same question now applies to the pancakes: the recipe card
    names a salted vanilla caramel, and the fact sheet uses that name.

13. **The spirit in the spiked Wild Pumpkin is still unnamed** in the CMS. If Bret
    asks what the $10.99 spike is, we need an answer from the bar.

## Assets

14. **No press-resolution stills for three items.** Gluten-free Pumpkin Pie
    Pancakes (784 × 758), The Wild Pumpkin (800 × 1249) and the Spicy Mary
    (800 × 1200) exist only at web resolution. Everything else is 3333 × 5000 or
    better. Chase Ed Aller for the originals.

15. **Spicy Mary hero shows a branded vodka bottle** in the background while the
    build specifies house vodka. Worth a look before that shot goes out for
    editorial use.

16. **Photo credit unconfirmed.** The fact sheet reads "courtesy Wild Eggs."
    Confirm whether Ed Aller requires a byline.

## Housekeeping

17. **Monday tracker is stale.** The SPICE SPICE BABY item still reads
    Sep 28 to Nov 22. The CMS has every item dated 2026-09-30 with
    "Sep 30 to Nov 24, 2026" in the nutrition block, and the live page agrees.

18. **Protein Bowl** was on the tasting sheet, never priced, and has no CMS
    record. Correctly excluded. No action unless it comes back.
