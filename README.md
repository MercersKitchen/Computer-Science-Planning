# Computer Science Planning
Intended for Teachers: Text Documents and Supporting Documents to begin imagining classroom experiences and projects-based learning

**Purpose**: jurisdictional & curriculum-level documents intended for project-based learning
- See Folder ABE Curriculum
  - CSE: intended for Computer Science Courses
    - Note: Website Outcomes overlap with previous "Communication Technologies" Curriculum Documents for Writing Websites
  - ELT: intended for "Physical Computing" (the coding side of robotics and physical interactions)
    - "Where the physical can make concrete the lines of code in a robotic app"
- Curriculum Level Documents called Courses in Computer Science Education of Alberta Education's Career and Technology Studies
- Curriculum Documents also from College Board's Advanced Placement: Computer Science Principles & Computer Pathways
  - See Folder AP CSA CSP

**Organization of Outcomes**: to facilitate industry-level, project-based learning
- See Folder ABE CSE
- "Thinking Like a Professional Developer": for example: web developer, production software developer for apps, etc.
  - Note: Develop Linked In Account for Part Time Jobs and Summer Internships
- Sections: Theory & Concepts, Algorithm, Data & Data Structures, and Coding (Algorithm Translation)

---

# Ideas to Include

Link: Computer Curriculum Documents, <a href="https://drive.google.com/drive/folders/117id1RIavhyMzYVW7_HPSVZg1DrGxqRa">Click Here</a>
- See Alberta Education Website for Related Downloads

Link: Course Outlines, <a href="https://drive.google.com/drive/folders/1pEr3PWr12lc5OEj-lAOXBSp5x6kT2ELK">Click Here</a>

Website Development
- Build Personal Home portfolio for our Adventures (Try to develop templates)
- Google's New Core Web Vitals: https://paper-leaf.us2.list-manage.com/track/click?u=ed9a96e3d5b0c7631056ad16c&id=4f752157c6&e=004b52e739
- Include other ways of testing websites (see Becky's Videos)
- See: https://www.youtube.com/watch?v=0-S5a0eXPoc&feature=youtu.be
- See: Mosh React Native Course
- Other reading
  - https://webmasters.googleblog.com/2020/05/evaluating-page-experience.html
  - https://blog.chromium.org/2020/05/introducing-web-vitals-essential-metrics.html
  - https://paper-leaf.com/blog/2016/06/user-centered-design-makes-everyone-happier/
  - https://chrome.google.com/webstore/detail/web-vitals/ahfhijdlegdabablpippeagghigmibma
  - https://developers.google.com/speed/pagespeed/insights/
  - https://paper-leaf.com/services/design-build/website-design-development/
  - https://paper-leaf.com/services/strategy-consultation/website-audit/

Reminder: Processing-JAVA syntax error
- Sometimes Processing-JAVA's debugger will describe a syntax error that is not true
- Solution:
  - Open new processing-java program
  - copy code to Notepad.txt (deletes all hidden formatting tags)
  - copy from Notepad.txt to new Processing.pde file (including creating any TABs
- Test new Processing.pde file to ensure formatting tags are *not* copied over

Interesting Problem that applies to visual data
- not overlapping rectangles, see partial solution below
```java
int obsticles = 2;
int[] x = new int[obsticles];
int[] y = new int[obsticles];
int[] rectWidth = new int[obsticles];
int[] rectHeight = new int[obsticles];

void setup() {
  size (500, 500);
  for (int i=0; i<=obsticles-1; i++) {
    // Choose Coordinates of first rectangle, parameters of rect()
    int a = i;
    x[i] = int (random (0, 501) );
    y[i] = int (random (0, 501) );
    rectWidth[i] = int (random (x[i], width-x[i]-1) );
    rectHeight[i] = int (random (y[i], height-y[i]-1) );
    if (i>0) { //test for overlap of next values
      //Bigger or Smaller than entire rectangle
      for (int j=a; j<=0; j--) {
        if (x[i] > x[i-1]+rectWidth[i-1]) { //Empty IF
        } else if (x[i] < x[i-1]) { //Empty IF
        } else {
          x[i] = int (random (0, x[i-1]-1) );
          while (x[i]+rectWidth[i] > x[i-1]) {
            rectWidth[i] = int (random (0, x[i-1]-1) );
          }
        }
        if (y[i] > y[i-1]+rectHeight[i-1]) { //Empty IF
        } else if (y[i] < y[i-1]) { //Empty IF
        } else {
          y[i] = int (random (0, y[i-1]-1) );
          while (y[i]+rectHeight[i] > y[i-1]) {
            rectHeight[i] = int (random (0, y[i-1]-1) );
          }
        }
      }
    }
  }

  //println (x, y, rectWidth, rectHeight);
}

void draw() {
  for (int i=0; i<=obsticles-1; i++) {
    rect (x[i], y[i], rectWidth[i], rectHeight[i]);
  }
}

```
---
