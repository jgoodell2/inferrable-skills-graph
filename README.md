# Learning Pathway Graph

### Diagram
![Competency graph demo image for readme md](https://github.com/user-attachments/assets/1da65250-b1a6-4b6f-9ac2-cda5cba8bce1)

## ItemSim: Fraction Problem Response Simulator

The ItemSim application (`itemsim.html`) allows users to:
- Enter responses to fraction-based problems 
- Simulate that the problems are practice for 5 different competencies using a dropdown 
- Submit answers for evaluation
- Store results automatically in the Learning Record Store (LRS) as attempts at demonsating a competency
- Track learning progress over time
- This formative assessment simulation is hardcoded with items representing 5 competencies/skills
- Logging in the xAPI LRS is hardcoded to a single fake student user id

### How to Use ItemSim
1. Open `itemsim.html` in your browser
2. Select a competency to simulate from the dropdown (The URI of the competency will be shown)
2. Complete the fraction problems presented 
3. Click "Check Answer" to evalute and log the response (You can answer more than once to create data, e.g. hit "Check Answer" multiple times.)
4. Results will be automatically recorded in the LRS

## Demo: Competency Graph Analyzer

The Demo application (`demo.html`) provides:
- Interactive competency graph visualization based on the IEEE SHared Competency Definition standard (1484.20.3)
- Real-time prediction of succes on next attempt using a basic INFERable inference detector
- Predictive analysis for each competency node is displayed

### How Demo Works
1. Displays interactive graph interface using data from competencyData.json
2. Connects to the inference detector
3. Iteratively processes each competency node
4. Generates predicted values for all nodes
5. Displays results in a visual graph format
6. Both itemsim.html and demo.html are temporarily hard coded to the development team's LRS. It will need to be modified to implement a different LRS. And the new LRS connection deatils passed to INFERable for the inference requests. 

### Technical Requirements
- Modern web browser with JavaScript enabled
- Connection to SQL LRS
- Access to inference detector service
---
*For more information, please contact the development team.*
