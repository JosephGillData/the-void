There is:
* [[What is run on the CPUs at data centres (software)]]
* [[How these data centres physically operate (hardware)]]
* [[Who builds, maintains and operates the data centres]]
* [[Who owns the data centres]]
* [[Government, Defence & Societal Concerns]]
### Data Centre Power Supply
For whatever it is that the data centres do, they need electricity. That is the life blood of the system, without which, nothing works. Therefore, one of the main design constraints of a data centre is a continuous supply of electricity. 
The key components of the electricity supply infrastructure are:
- Grid power → main electricity source
- UPS → short-term battery backup
- Generators → long-term backup
- PDU → distributes power to racks
![[data_center_power-4338651.webp|486]]

Under Normal Operation:
1. Electricity comes from the power grid
2. Power flows through UPS, charging the UPS batteries
3. Power is distributed via PDUs to racks of servers running continuously

Data centres and GPU clusters draw massive amounts of power, especially when training AI models. Power is the number one constraint in their design, which has limits on:
* Where the data centre (cluster) can be
* How big the cluster can be
### Power Supply Backups
Any disruption to the supply of power could cause the data centre to lose power, hence there are backups in place if energy sources are out.
#### Scenario: Power cut
* Grid power cuts out.
* UPS batteries instantly take over.
* The diesel engine generators are fired up, taking ~10 seconds.
* When the generators are active, the load is transferred from the UPS to the generators.
* The UPS returns to standby (recharging) and the data centre runs on the generator power until the grid is back up.
#### Scenario: Power cut + backup failure
* Grid fails, UPS activates, and the generator critically fails.
* UPS batteries last 5-15 mins.
* When UPS batteries run out, the systems begin emergency shutdown due to there being no power source.
* This causes a risk of data corruption, hardware stress and service outages.
* This has a real world impact of cloud storage issues, financial systems down, and AI workloads interrupted during training.

### System Design Trade Offs
#### Cost vs Redundancy
Running a data centre to make a profit requires balancing the design constraints, two of which are cost (energy use) and redundancy (having backups).
There are different approaches to this:
* N: No backup system. Cheap and high risk.
* N+1: One balanced backup system. Usual approach.
* 2N: A fully duplicated copy. Expensive, used for critical infrastructure.
#### Battery vs Generator
* UPS (battery): instant response, short duration.
* Generators: Slower start-up, long duration (fuel dependent).
#### Reliability vs Complexity
* A complex system allows for more sophisticated backups.
* Simpler systems are more reliable, easier to mange and have less operational failure points.
#### Key Insights
* The goal is to ensure a constant supply of energy to the servers
* If the grid has lost power, there is a threat to the servers energy
* Back up systems in place: UPS to bridge the gap to the generators (main backup).
* Redundancy increases reliability but scales cost rapidly
- AI infrastructure is fundamentally constrained by available power.

### Points of discussion
##### Why can’t generators replace UPS entirely?


What happens if both grid power and generators fail?

Why is N+1 often preferred over 2N?

In AI workloads, why does power become a scaling limit?

What is the weakest point in the power chain?