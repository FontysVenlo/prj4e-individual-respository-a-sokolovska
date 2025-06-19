# Personal Development Plan


This document holds my personal development plan for documentation of my progress towards achieving Learning Outcomes 1 and 2 of Project 4 module. They are separated into two categories for better readability and consistency.

- [Learning Outcome 1](#lo1)
    - [Definition](#lo1)
    - [Plan](#plan)
    - [Log](#log)
    - [Success Criterias](#success-indicators)
    - [Summary](#evaluation-and-summary)
- [Learning Outcome 2](#lo2)
    - [Definition](#lo2)
    - [Plan](#plan-1)
    - [Summary](#summary)

----
| Abbreviation | Meaning |
|--------------|---------|
| LO | Learning Outcome |
| PW | Project Week |
| SOC | State Of Charge |


----

### LO1:
 *The student plans and executes a project in their track at level 2 of the HBO-i framework regarding autonomy and complexity, in an agile way.* </br>

In my own words: I want to develop amphious robot that resembles a duck, while focusing on two main activities: [realise](/images/hbo-software.png) and [advise](/images/hbo-hardware.png). Advising on hardware-interfacing means analyzing, selecting, and justifying hardware components to meet functional and safety requirements. This would provide a technical base for the design phase focused on requirements; realization on software layer suggests designing and implementing  embedded software that controls hardware in a multithreaded, event-driven system. Well-done realization would ensure properly working software system with integrity, security and system performance. The learning curve will involve hardware research (motor types, microcontrollers, power supply options, sensors), hardware assembly, C/C++ skills enhancing (real-time system response to outside factors, multithreading, smooth and precise components control, integrated safety features, etc).

----

#### Plan:
| Week | Task                  | Relevant artifacts |
|:----:|-----------------------|:-----------------|
|  1   | Project Introduction, familiarization with provided module information  | Project 4 module Canvas files, [Module Description](/documents/md_prj4_2025.pdf), etc |
|  2   | Brainstorming ideas, defining initial project requirements | [Ideas list](/images/brainstorm.jpeg)
|  3   | Refining project concept, finalizing initial specifications | [Initial project idea](https://github.com/FontysVenlo/prj4e-repository-group_e02/blob/main/doc/initial-project-idea.md)
|  4   | Drafting Personal Development Plan (PDP) v1 | |
|  5   | Theoretical initial research on potential hardware, identifying key technical constraints| [Personal Notes on Components](/documents/hardware-research.md) |
|  6   | Advising based on analysed requirements, first selected modules, parallel research of software architecture | [Hardware selection document](https://github.com/FontysVenlo/prj4e-repository-group_e02/blob/main/documentation/GreatComponentList.md) |
|  7   | Project charter finalization, similar products research |[Project Charter](https://github.com/FontysVenlo/prj4e-repository-group_e02/blob/main/documentation/Project4-charter-02.md)
|  PW1 | Basic hardware building, outer frame, basic software implementation,  RC car autopsy | [RC car review](/documents/rc-car.md)  |
|  PW2 | Hardware work, first rough prototype with approximate final weight, mostly focusing on wheels structure | [Weight calculations](/documents/weight-calculations.md), [Weight test - video](/video/weight_test.mp4) |
|  8   | Focus on more in-depth software implementation and combining modules together | [Electrical circuit layout V1](https://github.com/FontysVenlo/prj4e-repository-group_e02/blob/dev/documentation/images/circuit_image.svg) |
|  9   | Propulsion system further research and implementation including typical motor connectors | [Notes on Propulsion](/documents/propulsion-system.md) |
|  10  |  Reworking electical circuit with consideration of extra power source and ON/OFF button |  [Electrical Circuit Layout V2 and V3](https://github.com/FontysVenlo/prj4e-repository-group_e02/blob/dev/documentation/images/circuit_image_v3.svg)  |
|  11  | Integrate hardware and software subsystems and test functional connections separately (movement, sensors, sound) | [Motor test - photo](/images/photos/separate_motor_testing.jpeg), [Propulsion assembly check - video](/video/propulsion_first_assembly.mp4) |
|  PW3 / 12  | Motor tuning for movement precision, components interaction testing, assembling and testing full propulsion system | [Better circuit documentation](https://github.com/FontysVenlo/prj4e-repository-group_e02/blob/main/documentation/circuit.md), [Component Interaction test - video](/video/component_interaction_test.mp4) |
|  PW4 / 13  | Final preparations of the outer frame and electical circuit | [Electrical Circuit V4](https://github.com/FontysVenlo/prj4e-repository-group_e02/blob/dev/documentation/images/circuit_image_v4.svg), [Outer Frame Preparation - photo](/images/photos/outer_frame_prep.jpeg) |
|  PW5 / 14  | Full assemble and testing in different enviroments with proper documentation and safety measures | [First Water test - video](/video/first_water_test.mp4), [Obstacle Avoidence test - video](/video/water_test_obstacle.mp4), [Final Electrical Circuit V5](https://github.com/FontysVenlo/prj4e-repository-group_e02/blob/main/documentation/images/circuit_image_v5.svg) |


**Examples of LEARNING MATERIAL can be found [here](/documents/learning-material.md)**

--------
#### Log:

The project began in **Week 1** with orientation. We familiarized ourselves with the scope and expectations.

Relying on that information, in **Weeks 2 and 3**, we [brainstormed ideas](/images/brainstorm.jpeg) and selected one of them, focusing on the scope and [initial requirements](https://github.com/FontysVenlo/prj4e-repository-group_e02/blob/dev/documentation/initial-project-idea.md). Interestingly, some of the more “wild” ideas later turned out to be surprisingly useful.

I drafted my first **PDP** in **Week 4**, but had to revise it a couple of times after realizing my goals were defined too vague.

The main work phase began in **Weeks 5 and 6**, when I launched initial [research into hardware](/documents/hardware-research.md). I struggled at first due to limited knowledge and time pressure, but soon I began contributing suggestions for [components](https://github.com/FontysVenlo/prj4e-repository-group_e02/blob/dev/documentation/GreatComponentList.md) and felt more confident explaining my reasoning and proposing alternatives.

Meanwhile, we were also working on the [project charter](https://github.com/FontysVenlo/prj4e-repository-group_e02/blob/dev/documentation/Project4-charter-02.md), which we finalized in **Week 7** after long discussions about the intended scope and prioritization of functionality.

In **PW1**, the first components were delivered. We began preparing the frame and getting used to working with embedded components—both hardware and software. I also [dissasembled similiar product](/documents/rc-car.md) to get more ideas.  Since key parts like the motors and batteries arrived late, **PW2** was spent [testing](/video/weight_test.mp4) the prototype under [estimated full weight](/documents/weight-calculations.md) and designing [water wheels](https://github.com/FontysVenlo/prj4e-repository-group_e02/blob/dev/documentation/3dPrint/Waterwheel_v2.1.stl) for 3D printing—despite no one on the team having prior 3D modeling experience.

In **Week 8**, our focus shifted to software integration and the [first circuit draft](https://github.com/FontysVenlo/prj4e-repository-group_e02/blob/dev/documentation/images/circuit_image.svg). Debugging the compass module was especially challenging for me due to interference from other components and a lack of clear feedback, but the process turned into a valuable learning experience.

In **Week 9**, we focused on attaching the motors to the frame while trying to maintain maximum waterproofing. With motors finally mounted, we began working on the [attachment of the wheels](/documents/propulsion-system.md). Unfortunately, I burned one of the motors during connection but managed to get a replacement the following week.

From **Week 10**, after long discussions with stakeholders, we agreed to use two separate power sources—one for the controller and modules, and another for the motors. This decision added a number of unexpected tasks and required significant changes to the electrical circuit, which resulted in [version 2](https://github.com/FontysVenlo/prj4e-repository-group_e02/blob/dev/documentation/images/circuit_image_v2.svg) and [version 3](https://github.com/FontysVenlo/prj4e-repository-group_e02/blob/dev/documentation/images/circuit_image_v3.svg) with proper switch ON/OFF mechanism.

**Week 11** was dedicated to subsystem testing after the circuit rework and early preparations for the [low battery detection](/documents/battery-level.md) feature, which introduced AD conversion and hence, [version 4](https://github.com/FontysVenlo/prj4e-repository-group_e02/blob/dev/documentation/images/circuit_image_v4.svg) of the circuit.

Finally, during **PW3–PW5**, we integrated everything, tuned performance, and implemented the low battery behavior. Late advice about adding fuses led to a last-minute [redesign of the circuit](https://github.com/FontysVenlo/prj4e-repository-group_e02/blob/main/documentation/images/circuit_image_v5.svg) and final assembly — but resulted in safer and more complete system. At last, we [successfully tested](/video/water_test_obstacle.mp4) the system in the pond with all components proving to be working as inteded. 


--------

#### Success Indicators:


- A structured project plan with agile methodologies.
- A clear technical documentation for hardware and software implementation.
- Documented progress with explained choices.
- Successfully implemented and tested both software and hardware.
- Constructive feedback from team members and coaches.
<br>

------

#### Evaluation and summary:
Over the course of the project, I’ve grown significantly in both preparing and executing technical tasks within an agile team. By focusing on hardware advising and software realization, I improved my ability to make technical decisions, justify them and build functional embedded systems. Despite component delays, limited hardware experience, and last-minute design changes, I adapted quickly and contributed consistently

This project not only improved my technical skills in C++, multithreading and embedded building, but also helped me gain experience which can easily be reused in the future projects. Looking back, despite relatively narrow scope of this project, I have acquired knowledge in main basic embedded topics such as hardware selection, building and integration with software, meaning I can do further similiar projects way faster and in a more efficient way. Extended version of reflection can be found [here](/documents/reflection.md).

-----
<br>
<br>

### LO2:
*The student demonstrates professional skills at level 2 in the focus areas: future-oriented organization, investigative ability, personal leadership, and targeted interaction.*

For Learning Outcome 2, I aim to strengthen my soft skills by developing better perspective awareness, setting clear and realistic goals, and improving how I communicate in various contexts. 

To make this goal concrete and measurable:
- Perspective awareness: I will regularly seek feedback and reflect on it. This will help me recognize different viewpoints and adjust my further approach accordingly.

- Goal setting: I will set weekly goals at the start of each project week and review them at the end of the week to assess completion. These goals will be specific and directly linked to both in-andout-project deliverables.

- Time management: I will aim to be on time for project sessions on all occasions. Additionally, for time management of deadlines, I will keep buffer time for unexpected delays, with the aim of submitting all individual contributions at least 24 hours before the team’s deadlines.

- Communication: I will actively contribute to team discussions. I also aim to take on the responsibility of documenting most feedback and results from team meetings.

- Investigative ability: I will conduct background research on at least three relevant technologies before proposing solutions and document these in the personal research notes.

Through this approach, I want to become more intentional and effective in  planning, researching, interacting, and leading throughout this project—building a mindset that balances technical depth with interpersonal awareness.

----
#### Plan:

| Week | Focus Area | Tasks | Relevant sources |
|:----:|------------|-------|:-----------------|
|  4   | Future-Oriented Organization | Define personal goals and ways for professional development | PDP v1, [Personal Goals](/documents/personal-goals.md) |
|  5   | Investigative ability | Research project-relevant practices in hardware | [Personal notes on hardware](/documents/hardware-research.md)  |
|  6   | Targeted Interaction | Seek feedback, reflect on the past weeks | [Documented Feedback](/documents/feedback.md), [Reflection Weeks 1-6](/documents/reflection.md)  |
|  7   | Personal Leadership | Organize work distribution and ensure the completion of project charter in-time  | [Project Charter](https://github.com/FontysVenlo/prj4e-repository-group_e02/blob/main/doc/Project4-charter-02.md)|
|  8  | Future-Oriented Organization | Review mid-project progress and adjust further plan accordingly | [Group](https://github.com/orgs/FontysVenlo/projects/618/views/1) and [Individual](https://github.com/orgs/FontysVenlo/projects/598) Project Boards, [Retrospective meeting log](https://github.com/FontysVenlo/prj4e-repository-group_e02/blob/dev/documentation/retrospective-results.md) |
|  9  | Investigative Ability | Explore different options for connection of propulsion system, motor connectors in particular | [Propulsion System Notes](/documents/propulsion-system.md) |
|  10 | Targeted Interaction | Discuss acquired information with the team and stakeholders, consider alternatives | [Feedback](/documents/feedback.md) |
|  11 | Future-oriented Organization | Reorganize and update individual documentation, brainstorm tasks for the following project weeks | [Reflection Weeks 6-11](/documents/reflection.md), [Kanban board](https://github.com/orgs/FontysVenlo/projects/618/views/1), |
|  12 | Personal Leadership | Lead the hardware circuit building, distribute tasks | [Circuit versions](https://github.com/FontysVenlo/prj4e-repository-group_e02/tree/dev/documentation/images) |
|  13 | Investigative Ability | Ensure proper documentation for the circuit | [Circuit instructions and version history](https://github.com/FontysVenlo/prj4e-repository-group_e02/blob/dev/documentation/circuit.md)
| 14 | Future-oriented Organization | Evaluate and reflect on project's process | [Reflection Weeks 12-14](/documents/reflection.md)


-----
#### Summary:

Throughout this project, I have made a good progress in strengthening my professional skills in comparision to the beginning of the semester. I regularly set clear and realistic weekly goals, which helped me keep track of planning and mantain a structured approach while staying focused on both technical and personal development. By actively seeking and documenting feedback from stakeholders, I improved my ability to look at the given situation from a different perspectives and became way more adaptive in my interactions with teammates and stakeholders.

I practiced investigative ability by conducting multiple targeted research on hardware option, propulsion systems and battery's SOC before making decisions, ensuring they were explained with proper technical reasoning. Taking on responsibilities like documenting team discussions and organizing retrospectives helped me improve in personal leadership and communication. Toward the end of the project, I also led circuit-building and overall hardware handling efforts, further enhancing these competencies.

Overall, I became more intentional in managing my time, responsibilities and interactions. It balances with individual technical growth ensuring improvement in all four focus areas of the needed soft skills: future-oriented organization, investigative ability, personal leadership, and targeted interaction. Of course, while overall progress is clearly there, there are parts of processes that could have been done in a better and more efficient way. More about it in [reflection](/documents/reflection.md).