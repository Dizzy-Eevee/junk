# Phase 1: Give Librarian Library Mechanics

- Add a library database computer that can scan books to register them to the database
	- Scanning an ID card followed by an arbitrary number of books allows books to be lended out to crew, with an optional time limit (so the librarian can harass crew about overdue books)
	- Computer functions as combined console and server; destroying the console will wipe the database.
- Add a librarian locker that spawns with a handheld tablet-computer-thing that facilitates easier registration and lending of books. 
	- Handheld will be a thief objective.
- Port the Impstation book teleporter, which periodically teleports in new books for the Librarian to catalogue.
	- Do *not* include Imp’s librarian spellbooks.
  
Requires mapping changes, obviously. I don’t see this suddenly making Librarian wildly popular, but it’s always nice to have mechanics to complement your roleplay, and it establishes things that will be useful in the next phase.

# Phase 2: Book Restoration


- Adds ruined books, which can be found in salvage loot tables, and occasionally included in book teleporter shipments. 
	- Ruined books are worth (tentatively) 250 spesos when sold directly, but should be turned in to the Librarian to be restored for better profits.
- Ruined books fall into three categories:
	- Monographs, which function as research discs worth (tentatively) 1000-5000 research points.
	- Novels, which can be sold for (tentatively) 1000-5000 spesos.
	- Tomes, minor magical artifacts that range from moderately useful tools to silly gag items.
- Books can be analyzed using a magnifying glass which spawns in the Librarian’s locker. The magnifying glass will show the damages that need to be repaired, the book’s attributes which will determine the outcome of identification, and is used to finalize the process and identify the book.
	- Traitor Librarians can purchase an enchanted Scrying Glass for 12(?) TC, which can be used to “subvert” identified tomes into more powerful (and highly illegal) magical tomes.
- Books spawn with random damages applied that must be “healed” before being identified. These fall into 4 “tiers”, e.g. “the book’s pages are lightly/moderately/severely/extremely stained”, with each tier requiring one use of a repair item.
- Books are restored with a set of reagent-fueled tools (mechanically similar to a welding tool)
	- Damaged binding, repaired with a book binding kit (consumes 5u space glue per use)
	- Stained pages, repaired with a page cleaning swab (consumes 5u bleach per use)
	- Torn pages, repaired with a page repair kit (consumes 5u flour per use (as a stand-in for starch))
	- Dirty cover, repaired with a book cleaning kit (consumes 5u ethanol per use)
	- {todo?}
- Tomes generate with a combination of “arcana”, which are used to determine the outcome of identifying a tome. Arcana can be altered using a special tool fueled by solid plasma.
	- An artifact’s “recipe” is an up-to-16-digit sequence of arcana. This sequence is place-insensitive, but all required arcana must be adjacent and in the correct order. (i.e. a 4-digit recipe can be crafted with 12 leading Null arcana, followed by the 4 required arcana).
	- Altering an arcana requires 1 sheet of solid plasma. 
	- Tomes should generate with a valid, left-aligned recipe for a lesser artifact. Greater artifacts will require sequence editing and thus plasma, serving as a further obstacle for bulk production of antag items.    
	- A recipe's length should generally correspond to the strength of the artifact; things with stronger effects or more practical applications should require more plasma to manually create to limit their acquisition.
	- There are 16 arcana:
		1. Null (acts as an empty space)
		2. Gaia (earth, plants, nature undisturbed)
		3. Mist (water, ice, cold)
		4. Pyre (fire, light, heat)
		5. Zephyr (wind, weather, transience)
		6. Flesh (life, hunger)
		7. Entropy (decay, chaos, random chance)
		8. Bluespace (size, space)
		9. {}
		10. {}
		11. {}
		12. {}
		13. {}
		14. Blood (nar’sie, violence)
		15. Clockwork (ratvar, time, metal)
		16. Honk (clowns, silly stuff, gag items)
	- {todo}
# Lesser artifact ideas
- Tome of {x}light
	- Functions as an unlimited glowstick of the specified color.
	- Should generally use colors that are purposefully inconvenient and provide worse visual clarity, similar to the glowstick’s extremely aggressive green light. These should be desirable for the lack of power management, but strictly worse than a flashlight or lamp with a microreactor.
	- Has two rare variants:
		- Tome of Rainbows/Tome of Gamerlight (probably too goofy to make the cut lmao); simply an infinite glowstick with the rainbow light component
		- Tome of Unlight; inverts the colors of everything within its radius. Will most likely require custom shaders, might be too visually obnoxious to make the cut, but I think it’s a cool idea.
- RGB Book / RGBook?
	- Functions like the RGB staff.
- Book of Soap
	- It’s a slippery book. The clown will probably want it.
- Tome of {x} Familiar
	- Summons a spectral variant of a “pet” mob (e.g. cat, mothroach, etc) that follows the user and is available as a ghost role. 
    - Each book can only summon one familiar
    - Familiars can be recalled or resummonned using an ability
	    - Ideally this should not remove the ghost role.
    - Familiars take no damage and are spaceproof, but also deal no damage. They’re just there to be cute.
	    - Should also not be attacked by any hostile mobs
	- No limit on the number of peaceful familiars you can have at once. Go forth and conjure your phantom mothroach army.
- Book of Song / Songbook / ??
	- Gag instrument, maybe a blunt impact sound, as if you’re playing music by smacking it against things?
- {Cleaning book}
	- Instant space cleaner foam. Smaller area than a proper cleanade; 1-3 charges with a moderately lengthy cooldown
    - Cooldown mainly exists as a nerf for antagonists, instant cleanade could be abused as an escape tool.
    - No recharge because we don't want librarians putting janitors out of a job.
- {some form of edible book}
- {harmless polymorph spells?}
	- like, cat polymorph. probably no need for limited duration or charges, just don't make it anything that can go under doors or has substantial combat viability
- {todo}
# Greater artifact ideas
The upstream ones:
- {Knock spellbook}
	- Opens locks/doors within 10 tiles and LoS.
	- 2 charges, 10s cooldown, 1min recharge?
	- kinda like a magical access breaker
- {Blink spellbook}
	- Teleports you to where you click, provided you have LoS.
	- 2 charges, 10s cooldown, 180s recharge?
- {Spawn spellbook}
	- Summons 3 magicarp. 
	- Shouldn't be too bad, especially if they're hostile to the user too.
	- I was initially considering that this should be nerfed heavily but fuck it carpbombing is funny
	- 3 charges, 2s cooldown, no recharge
- {Force wall spellbook}
	- Summons a line of 3 barriers in front of the user that are passable to them, but impassable to everyone else
	- 2 charges, no recharge
- {Entrance spellbook}
	- Like upstream wand of entrance, but in book form.
	- Maybe make it a touch spell rather than a "gun"?
	- 1-3 (undecided) charges, non-recharging.
- {Repulse spellbook}
	- Smaller radius than wizard repulse. 
	- 1 charge, 5min recharge?
- {Smoke spellbook}
	- Probably fine without nerfs. 
	- 1 charge, 5min recharge?

We're not doing smite. Don't even ask.
Spider polymorph, or other polymorph spells, could be cute.
Fireball might be okay as a high-arcana tome with 1 non-renewing charge
Mindswap might be acceptable as a 16-arcana tome. Unlike wizards, none of your abilities are innate, so you'll be leaving all your antag equipment with your original body.
Void applause is a maybe, though it'd need retheming to work as a book.

Original stuff:
- Magic Missile
    - Ranged weapon with a small pool of regenerating ammo. Ideally should be worse than a Viper in a sustained fight, but still good enough to kill someone in maints with.
	    - Deals a mix of pierce and heat?
	    - Maybe a red/blue/purple variant that do heat/cold/shock respectively?
- Tome of {x} Familiar
	- Summons a very real variant of a combat-inclined mob that is hostile to all non-Syndicate mobs, and is available as a ghost role.
    - For obvious reasons, these should not be summoned immediately like the “pet” familiars are.
    - Takes and deals damage as normal, cannot be resummoned once killed.
    - Ideally these should be hostile to anyone but the user. Maybe add a second ability to register nonhostiles? 
	    - Would prefer to not use pre-existing factions, so tots can team up with non-Syndie antags and not worry about their familiar killing them.
	- Maybe limit the user to a single combat familiar to prevent carpbombing strats, funny as they are
	- Add rat-king-like commands for AI familiars
- {Healing circle spellbook}
	- Idea credit to saintly
	- Places down a glowing spell circle that slowly heals anyone inside it. 
	- Implementation idea A:
		- Use to deploy/undeploy under your feet
		- 2x2 decal that even heals all damage at 5/s.
			- Should be large enough to be able to comfortably heal allies
		- Can heal up to {100? 200? 400?} damage in total. 
			- Once charge is depleted, the circle turns inert and the tome can no longer be used.
				- Inert tome can be removed with space cleaner.
- {flash}
	- 1 charge, 1min recharge?
	- useless against sec but possibly useful against targets
	- make it have harmflash too
		- shoving the book in their face like uncle ruckus
- {book that gives you a remote explosive charge and a spell ability that activates it} 
	- 3 second minimum timer?
- {todo}