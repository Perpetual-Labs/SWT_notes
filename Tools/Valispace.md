"Github for Hardware"
Similar software: [[CDP4]]
Based on: [[Octave]]

From Valispace Tutorials

For use on complex hardware:
 - budget overruns and schedule slips are common
 - so provide home for digital data			
				
Valispace:
 - browser-based tool
 - complements existing tool landscape
 - enables lean engineering
 - automatic data exchange across tools and documentation
 - less time chasing design statuses, digging through documents, cross-referencing data
 - "collaboration platfrom where you can calculate and store your engineering data"			
	
Reasons to use Valispace:
 - Today, all your engineering calculations are done in isolated [[Excel]] sheets which are not connected
 - You want to solve an engineering problem and be able to save the history and share your work
 - Your team needs a central data storage with always up-to-date values
 - You want to be notified automatically when someone changes a design value		
				
Valispace Introduction Video:
 - Valispace web browser interface
 - Connected Valispace to analysis in [[Python]]
 - e.g. update mass with 10% margin
 - automatically proprgates values through to requirements, and other dependents
 - automatically propagates values through to reports
 - can generate charts, etc. in reports
 - can have a Valispace plug-in to Microsoft Word			
				
Workspaces:
 - are isolated, can't share value,s etc. between them
 - Can see project overview, timelines, etc.

Components and Valis:
 - Components (similar to blocks) - physical parts of the product
 - Valis - parameters of components
 - Valis have shortnames, names, values, margins, formulae, units, min/max
 - Users can subscribe to valis to be notified every time they change
 - Components don't need to be physical - e.g. Orbit, Mission (raises question of ontology)
				
Analysis Module:
 - Link valis to reports, automatically updated
 - Add 'blocks' (like subsections of report) to report
 - e.g. text, image, charts, tables
 - Can download reports as pdf or share by link

Timelines:
 - Next release, can specific mode transitions by time and event (e.g. battery <30%)

Requirements Module:
 - Store, filter and assign requirements to your project's components
 - Track verification statuses and compliances throughout the design phases
 - Subscribe to requirements to be notified when they are changed
 - Manage child requirements
 - Can set 'verified by' to test, then will automatically be verified when test is complete

Test Procedures:
 - Can link to requirements (next release, Jan)
 - Automatic verification
				
Simulation Module:
 - Connects input and output Valis
 - Uses the 'GNU [[Octave]]' framework - so very similar to [[MATLAB]] (.m) files, and is compatible
				
Cool features:
 - Link to data sets to find values
 - Import requirements from [[DOORS]], [[Excel]]
 - Can have multiple verification strategies for requirements - e.g. add rules
 - Can have containers to compare different components (e.g. types of battery)
 - Link budget values to different modes
 - Automatically generate reports, etc.
 - Create tasks and discussions
 - Subscribe to certain values
 - It does integrate with AGI [[STK]] (via plugin) - can sync values and data sets across STK and Valispace - looks neat
 - History - previous values of Valis stored in a database, with a change log (like Git)	
				
Things it can't do:
 - Functional stuff - no FFBD or STM diagrams
 - Operational stuff - same as above
 - It is quite prescriptive
 - Multivariate analysis - may be possible to run programmatically via [[Python]] API?
 - Connected Copies - can't match components but different modes (i.e. for redundant components)


Reference: Valispace Tutorials (only two available currently)
Reference: [[Meeting - 201221]]
