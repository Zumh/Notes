- ## Importance of Prerequisties
  collapsed:: true
  ((63f28afb-6311-47f1-a968-169d7e2ce18b))
	- A common denominator of programmers who build high-quality software is their use of high-quality practices.
	- Such practices emphasize quality at the beginning, middle, and end of a project.
	- ## Boss-Readiness Test
		- We've investigated requirements and design so much that I can't think of any major problems we'll run into during coding or debugging.
	- ## Determine the Kind of Software You're Working On
	  ((63f3dd9b-e720-4ece-afe3-051f109c2d90))
		- Business Systems
			- benefit from highly iterative approaches, in which planning, requirements, and architecture are interleaved with construction, system testing, and quality-assurance activities
		- Mission Critical Systems
			- sequential approaches— requirements stability is part of what's needed to ensure ultrahigh levels of reliability
		- Embedded Life-Critical Systems
			- sequential plus requirement
		- Rule of thumb
			- One common rule of thumb is to plan to specify about 80 percent of the requirements up front, allocate time for additional requirements to be specified later, and then practice systematic change control to accept only the most valuable new requirements as the project progresses.
			- Another alternative is to specify only the most important 20 percent of the requirements up front and plan to develop the rest of the software in small increments, specifying additional requirements and designs as you go.
	- ## Choosing Between Iterative and Sequential Approaches
	  ((63f3ddb7-43e1-4d8a-8db4-897d1c5947a1))
		- ## Sequential
			- The requirements are fairly stable.
			- The design is straightforward and fairly well understood.
			- The development team is familiar with the applications area.
			- The project contains little risk. Long-term predictability is important.
			- The cost of changing requirements, design, and code downstream is likely to be high.
		- ## Iterative Approach
			- The requirements are not well understood or you expect them to be unstable for other reasons.
			- The design is complex, challenging, or both.
			- The development team is unfamiliar with the applications area.
			- The project contains a lot of risk.
			- Long-term predictability is not important.
			- The cost of changing requirements, design, and code downstream is likely to be low.
- ## Problem-Def Prerequisite
  ((63f3dfee-e0e9-4837-854e-a38add6d7776))
	- Problem definition lay foundation of programming process
	- User language and problem described user's point of view
	- "Find the box first before thinking outside of the box" Andy Hunt Dave Thomas
- ## Requirements Prerequisite
  ((63f7abba-4131-45a9-abfc-4f6c1b6878df))
	- Explicit requirements help to 
	  * ensure that the user rather than the programmer drives the system's functionality. 
	  * avoid arguments.
	  * time is expensive and we don't want to miss specific aspects of the problem.
- ## Myth of stable requirement
  ((63f7acb4-068d-44aa-b530-f6cfb39c6ef9))
	- Requirement is like water if frozen easier to build
	- The development process helps customers better understand their own needs.
	- If customer change their mind during construction 
	  * make schedule for revised and estimated cost
	  * reality check for customers
	- An evolutionary prototyping approach help build system's requirements.
	  * build little, get a little feedback, adjust design a little, and few changes.
	- To dump or not to dump project
	  * if the benefit of quitting project out weight the result
	  * Clarify to customer because sometime requirement disappear.
- ## Requirement sanity check
  ((63f7af1e-01fa-4864-b6af-b995a4128bf4))
	- Are all the inputs to the system specified, including their source, accuracy, range of values, and frequency?
	- Are all the outputs from the system specified, including their destination, accuracy, range of values, frequency, and format?
	- Are all output formats specified for Web pages, reports, and so on?
	- Are all the external hardware and software interfaces specified?
	- Are all the external communication interfaces specified, including handshaking, error-checking, and communication protocols?
	- Are all the tasks the user wants to perform specified? Is the data used in each task and the data resulting from each task specified?
- ## Non Functional
	- Is the expected response time, from the user's point of view, specified for all necessary operations?
	- Are other timing considerations specified, such as processing time, datatransfer rate, and system throughput?
	- Is the level of security specified?
	- Is the reliability specified, including the consequences of software failure, the vital information that needs to be protected from failure, and the strategy for error detection and recovery?
	- Are minimum machine memory and free disk space specified?
	- Is the maintainability of the system specified, including its ability to adapt to changes in specific functionality, changes in the operating environment, and changes in its interfaces with other software?
	- Is the definition of success included? Of failure?
- ## Requirements Quality
	- Are the requirements written in the user's language? Do the users think so?
	- Does each requirement avoid conflicts with other requirements?
	- Are acceptable tradeoffs between competing attributes specified—for example, between robustness and correctness?
	- Do the requirements avoid specifying the design?
	- Are the requirements at a fairly consistent level of detail? Should any requirement be specified in more detail? Should any requirement be specified in less detail?
	- Are the requirements clear enough to be turned over to an independent group for construction and still be understood? Do the developers think so?
	- Is each item relevant to the problem and its solution? Can each item be traced to its origin in the problem environment?
	- Is each requirement testable? Will it be possible for independent testing to determine whether each requirement has been satisfied?
	- Are all possible changes to the requirements specified, including the likelihood of each change?
- ## Requirements Completeness
	- Where information isn't available before development begins, are the areas of incompleteness specified?
	- Are the requirements complete in the sense that if the product satisfies every requirement, it will be acceptable?
	- Are you comfortable with all the requirements? Have you eliminated requirements that are impossible to implement and included just to appease your customer or your boss?