# python-ABL-assignments.
0 to 10
# University Scholarship Allocation System
# 1. Problem Statement
Develop a Python program to allocate university scholarships based on students' aggregate marks, subject-wise minimum marks, attendance percentage, and family income. The system identifies eligible students, ranks them according to their aggregate marks, and resolves ties using predefined rules such as higher attendance and lower family income.
# 2. Algorithm
1. Start the program.
2. Read the number of students.
3. Enter each student's name, aggregate marks, subject marks, attendance percentage, and annual family income.
4. Check the eligibility criteria:
   - Aggregate marks ≥ 75%
   - Minimum mark in every subject ≥ 60%
   - Attendance ≥ 75%
   - Annual family income ≤ ₹2,50,000
5. Add eligible students to the scholarship list.
6. Rank students by:
   - Higher aggregate marks first.
   - If marks are equal, higher attendance first.
   - If both are equal, lower family income first.
   - If still tied, alphabetical order of name.
7. Display the eligible students and their ranks.
8. Display a message if no students are eligible.
9. Stop the program.
# 3. Flowchart (Mermaid)
```mermid
#chatgpt-mermaid-_r_tj_{font-family:-apple-system-body,ui-sans-serif,-apple-system,system-ui,"Segoe UI",Helvetica,"Apple Color Emoji",Arial,sans-serif,"Segoe UI Emoji","Segoe UI Symbol";font-size:16px;fill:rgb(13, 13, 13);}@keyframes edge-animation-frame{from{stroke-dashoffset:0;}}@keyframes dash{to{stroke-dashoffset:0;}}#chatgpt-mermaid-_r_tj_ .edge-animation-slow{stroke-dasharray:9,5!important;stroke-dashoffset:900;animation:dash 50s linear infinite;stroke-linecap:round;}#chatgpt-mermaid-_r_tj_ .edge-animation-fast{stroke-dasharray:9,5!important;stroke-dashoffset:900;animation:dash 20s linear infinite;stroke-linecap:round;}#chatgpt-mermaid-_r_tj_ .error-icon{fill:rgb(243, 243, 243);}#chatgpt-mermaid-_r_tj_ .error-text{fill:rgb(13, 13, 13);stroke:rgb(13, 13, 13);}#chatgpt-mermaid-_r_tj_ .edge-thickness-normal{stroke-width:1px;}#chatgpt-mermaid-_r_tj_ .edge-thickness-thick{stroke-width:3.5px;}#chatgpt-mermaid-_r_tj_ .edge-pattern-solid{stroke-dasharray:0;}#chatgpt-mermaid-_r_tj_ .edge-thickness-invisible{stroke-width:0;fill:none;}#chatgpt-mermaid-_r_tj_ .edge-pattern-dashed{stroke-dasharray:3;}#chatgpt-mermaid-_r_tj_ .edge-pattern-dotted{stroke-dasharray:2;}#chatgpt-mermaid-_r_tj_ .marker{fill:rgb(143, 143, 143);stroke:rgb(143, 143, 143);}#chatgpt-mermaid-_r_tj_ .marker.cross{stroke:rgb(143, 143, 143);}#chatgpt-mermaid-_r_tj_ svg{font-family:-apple-system-body,ui-sans-serif,-apple-system,system-ui,"Segoe UI",Helvetica,"Apple Color Emoji",Arial,sans-serif,"Segoe UI Emoji","Segoe UI Symbol";font-size:16px;}#chatgpt-mermaid-_r_tj_ p{margin:0;}#chatgpt-mermaid-_r_tj_ .label{font-family:-apple-system-body,ui-sans-serif,-apple-system,system-ui,"Segoe UI",Helvetica,"Apple Color Emoji",Arial,sans-serif,"Segoe UI Emoji","Segoe UI Symbol";color:rgb(13, 13, 13);}#chatgpt-mermaid-_r_tj_ .cluster-label text{fill:rgb(13, 13, 13);}#chatgpt-mermaid-_r_tj_ .cluster-label span{color:rgb(13, 13, 13);}#chatgpt-mermaid-_r_tj_ .cluster-label span p{background-color:transparent;}#chatgpt-mermaid-_r_tj_ .label text,#chatgpt-mermaid-_r_tj_ span{fill:rgb(13, 13, 13);color:rgb(13, 13, 13);}#chatgpt-mermaid-_r_tj_ .node rect,#chatgpt-mermaid-_r_tj_ .node circle,#chatgpt-mermaid-_r_tj_ .node ellipse,#chatgpt-mermaid-_r_tj_ .node polygon,#chatgpt-mermaid-_r_tj_ .node path{fill:rgb(222, 234, 251);stroke:rgb(83, 154, 248);stroke-width:1px;}#chatgpt-mermaid-_r_tj_ .rough-node .label text,#chatgpt-mermaid-_r_tj_ .node .label text,#chatgpt-mermaid-_r_tj_ .image-shape .label,#chatgpt-mermaid-_r_tj_ .icon-shape .label{text-anchor:middle;}#chatgpt-mermaid-_r_tj_ .node .katex path{fill:#000;stroke:#000;stroke-width:1px;}#chatgpt-mermaid-_r_tj_ .rough-node .label,#chatgpt-mermaid-_r_tj_ .node .label,#chatgpt-mermaid-_r_tj_ .image-shape .label,#chatgpt-mermaid-_r_tj_ .icon-shape .label{text-align:center;}#chatgpt-mermaid-_r_tj_ .node.clickable{cursor:pointer;}#chatgpt-mermaid-_r_tj_ .root .anchor path{fill:rgb(143, 143, 143)!important;stroke-width:0;stroke:rgb(143, 143, 143);}#chatgpt-mermaid-_r_tj_ .arrowheadPath{fill:rgb(143, 143, 143);}#chatgpt-mermaid-_r_tj_ .edgePath .path{stroke:rgb(143, 143, 143);stroke-width:1px;}#chatgpt-mermaid-_r_tj_ .flowchart-link{stroke:rgb(143, 143, 143);fill:none;}#chatgpt-mermaid-_r_tj_ .edgeLabel{background-color:rgb(252, 252, 252);text-align:center;}#chatgpt-mermaid-_r_tj_ .edgeLabel p{background-color:rgb(252, 252, 252);}#chatgpt-mermaid-_r_tj_ .edgeLabel rect{opacity:0.5;background-color:rgb(252, 252, 252);fill:rgb(252, 252, 252);}#chatgpt-mermaid-_r_tj_ .labelBkg{background-color:rgba(252, 252, 252, 0.5);}#chatgpt-mermaid-_r_tj_ .cluster rect{fill:rgb(243, 243, 243);stroke:rgba(0, 0, 0, 0.1);stroke-width:1px;}#chatgpt-mermaid-_r_tj_ .cluster text{fill:rgb(13, 13, 13);}#chatgpt-mermaid-_r_tj_ .cluster span{color:rgb(13, 13, 13);}#chatgpt-mermaid-_r_tj_ div.mermaidTooltip{position:absolute;text-align:center;max-width:200px;padding:2px;font-family:-apple-system-body,ui-sans-serif,-apple-system,system-ui,"Segoe UI",Helvetica,"Apple Color Emoji",Arial,sans-serif,"Segoe UI Emoji","Segoe UI Symbol";font-size:12px;background:rgb(243, 243, 243);border:1px solid rgba(0, 0, 0, 0.1);border-radius:2px;pointer-events:none;z-index:100;}#chatgpt-mermaid-_r_tj_ .flowchartTitleText{text-anchor:middle;font-size:18px;fill:rgb(13, 13, 13);}#chatgpt-mermaid-_r_tj_ rect.text{fill:none;stroke-width:0;}#chatgpt-mermaid-_r_tj_ .icon-shape,#chatgpt-mermaid-_r_tj_ .image-shape{background-color:rgb(252, 252, 252);text-align:center;}#chatgpt-mermaid-_r_tj_ .icon-shape p,#chatgpt-mermaid-_r_tj_ .image-shape p{background-color:rgb(252, 252, 252);padding:2px;}#chatgpt-mermaid-_r_tj_ .icon-shape .label rect,#chatgpt-mermaid-_r_tj_ .image-shape .label rect{opacity:0.5;background-color:rgb(252, 252, 252);fill:rgb(252, 252, 252);}#chatgpt-mermaid-_r_tj_ .label-icon{display:inline-block;height:1em;overflow:visible;vertical-align:-0.125em;}#chatgpt-mermaid-_r_tj_ .node .label-icon path{fill:currentColor;stroke:revert;stroke-width:revert;}#chatgpt-mermaid-_r_tj_ .node .neo-node{stroke:rgb(83, 154, 248);}#chatgpt-mermaid-_r_tj_ [data-look="neo"].node rect,#chatgpt-mermaid-_r_tj_ [data-look="neo"].cluster rect,#chatgpt-mermaid-_r_tj_ [data-look="neo"].node polygon{stroke:url(#chatgpt-mermaid-_r_tj_-gradient);filter:drop-shadow( 1px 2px 2px rgba(185,185,185,1));}#chatgpt-mermaid-_r_tj_ [data-look="neo"].swimlane.cluster rect{filter:none;}#chatgpt-mermaid-_r_tj_ [data-look="neo"].node path{stroke:url(#chatgpt-mermaid-_r_tj_-gradient);stroke-width:1px;}#chatgpt-mermaid-_r_tj_ [data-look="neo"].node .outer-path{filter:drop-shadow( 1px 2px 2px rgba(185,185,185,1));}#chatgpt-mermaid-_r_tj_ [data-look="neo"].node .neo-line path{stroke:rgb(83, 154, 248);filter:none;}#chatgpt-mermaid-_r_tj_ [data-look="neo"].node circle{stroke:url(#chatgpt-mermaid-_r_tj_-gradient);filter:drop-shadow( 1px 2px 2px rgba(185,185,185,1));}#chatgpt-mermaid-_r_tj_ [data-look="neo"].node circle .state-start{fill:#000000;}#chatgpt-mermaid-_r_tj_ [data-look="neo"].icon-shape .icon{fill:url(#chatgpt-mermaid-_r_tj_-gradient);filter:drop-shadow( 1px 2px 2px rgba(185,185,185,1));}#chatgpt-mermaid-_r_tj_ [data-look="neo"].icon-shape .icon-neo path{stroke:url(#chatgpt-mermaid-_r_tj_-gradient);filter:drop-shadow( 1px 2px 2px rgba(185,185,185,1));}#chatgpt-mermaid-_r_tj_ .node text{font-size:14px;font-weight:600;letter-spacing:normal;fill:rgb(0, 79, 153);}#chatgpt-mermaid-_r_tj_ .edgeLabels text{font-size:13px;font-weight:600;letter-spacing:-0.08px;fill:rgb(0, 79, 153);}#chatgpt-mermaid-_r_tj_ .node tspan[font-weight="normal"],#chatgpt-mermaid-_r_tj_ .edgeLabels tspan[font-weight="normal"]{font-weight:600;}#chatgpt-mermaid-_r_tj_ .edgeLabel .label rect{opacity:1;rx:13px;ry:13px;fill:rgb(245, 250, 255);stroke:rgb(206, 219, 229);stroke-width:1px;}#chatgpt-mermaid-_r_tj_ .node rect,#chatgpt-mermaid-_r_tj_ .node circle,#chatgpt-mermaid-_r_tj_ .node ellipse,#chatgpt-mermaid-_r_tj_ .node polygon,#chatgpt-mermaid-_r_tj_ .node path{fill:rgb(229, 243, 255);stroke:rgba(0, 0, 0, 0.1);stroke-width:1px;}#chatgpt-mermaid-_r_tj_ .node rect{rx:16px;ry:16px;}#chatgpt-mermaid-_r_tj_ .mermaid-decision .label-container{fill:rgb(245, 250, 255);stroke:rgb(206, 219, 229);stroke-dasharray:2,2;}#chatgpt-mermaid-_r_tj_ .edgePaths .flowchart-link{stroke:rgb(143, 143, 143);stroke-width:1px;stroke-linecap:round;stroke-linejoin:round;}#chatgpt-mermaid-_r_tj_ .marker{fill:rgb(143, 143, 143);stroke:rgb(143, 143, 143);}#chatgpt-mermaid-_r_tj_ :root{--mermaid-font-family:-apple-system-body,ui-sans-serif,-apple-system,system-ui,"Segoe UI",Helvetica,"Apple Color Emoji",Arial,sans-serif,"Segoe UI Emoji","Segoe UI Symbol";}StartEnter student detailsAggregate >= 75%,all subjects >= 60%,attendance >= 75%,income <= 250000?Add to eligible listMark as not eligibleMore students?Sort eligible studentsRank by marks, attendance,income and nameDisplay scholarship ranking
```
# source code
students = []
n = int(input("Enter number of students: "))

for i in range(n):
    print("\nStudent", i + 1)
    name = input("Enter name: ")
    aggregate = float(input("Aggregate marks (%): "))
    subjects = list(map(float, input(
        "Enter 3 subject marks: ").split()))
    attendance = float(input("Attendance (%): "))
    income = float(input("Annual family income (Rs): "))

    if (aggregate >= 75 and min(subjects) >= 60
            and attendance >= 75 and income <= 250000):
        students.append({
            "name": name,
            "marks": aggregate,
            "attendance": attendance,
            "income": income
        })

# Rank by marks, attendance, income, then name
students.sort(key=lambda s: (
    -s["marks"], -s["attendance"],
    s["income"], s["name"].lower()
))

print("\n--- SCHOLARSHIP RESULTS ---")

if students:
    for rank, s in enumerate(students, 1):
        print(f"{rank}. {s['name']} | "
              f"Marks: {s['marks']}% | "
              f"Attendance: {s['attendance']}% | "
              f"Income: Rs.{s['income']:.0f}")
else:
    print("No eligible students found.")
<img width="856" height="526" alt="image" src="https://github.com/user-attachments/assets/b88981e5-faed-4a19-adc6-154374e610f9" />

