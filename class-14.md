## read a:
### transformation:
- The **transform** property comes in two different settings, two-dimensional and three-dimensional. Each of these come with their own individual properties and values.

* he actual syntax for the transform property is quite simple, including the transform property followed by the value. The value specifies the transform type followed by a specific amount inside parentheses.


div {
  -webkit-transform: scale(1.5);
     -moz-transform: scale(1.5);
       -o-transform: scale(1.5);
          transform: scale(1.5);
}


* 2D Transforms:

1. 2D Rotate: he transform property accepts a handful of different values. The rotate value provides the ability to rotate an element from 0 to 360 degrees.Using a positive value will rotate an element clockwise, and using a negative value will rotate the element counterclockwise. 

2. 2D Scale :Using the scale value within the transform property allows you to change the appeared size of an element. The default scale value is 1, therefore any value between .99 and .01 makes an element appear smaller while any value greater than or equal to 1.01 makes an element appear larger.

3. 2D Translate: The translate value works a bit like that of relative positioning, pushing and pulling an element in different directions without interrupting the normal flow of the document. Using the translateX value will change the position of an element on the horizontal axis while using the translateY value will change the position of an element on the vertical axis.

4. 2D Skew: The last transform value in the group, skew, is used to distort elements on the horizontal axis, vertical axis, or both. The syntax is very similar to that of the scale and translate values. Using the skewX value distorts an element on the horizontal axis while the skewY value distorts an element on the vertical axis. To distort an element on both axes the skew value is used, declaring the x axis value first, followed by a comma, and then the y axis value.%p

- **Combining Transforms**:
It is common for multiple transforms to be used at once, rotating and scaling the size of an element at the same time for example. In this event multiple transforms can be combined together. To combine transforms, list the transform values within the transform property one after the other without the use of commas.

Using multiple transform declarations will not work, as each declaration will overwrite the one above it. The behavior in that case would be the same as if you were to set the height of an element numerous times.

- **Perspective**
In order for three-dimensional transforms to work the elements need a perspective from which to transform. The perspective for each element can be thought of as a vanishing point, similar to that which can be seen in three-dimensional drawings.

The perspective of an element can be set in two different ways. One way includes using the perspective value within the transform property on individual elements, while the other includes using the perspective property on the parent element residing over child elements being transformed.

* 3D Transforms:

1. 3D Rotate: So far we’ve discussed how to rotate an object either clockwise or counterclockwise on a flat plane. With three-dimensional transforms we can rotate an element around any axes. To do so, we use three new transform values, including rotateX, rotateY, and rotateZ.

Using the rotateX value allows you to rotate an element around the x axis, as if it were being bent in half horizontally. Using the rotateY value allows you to rotate an element around the y axis, as if it were being bent in half vertically. Lastly, using the rotateZ value allows an element to be rotated around the z axis.

2. 3D Scale
By using the scaleZ three-dimensional transform elements may be scaled on the z axis. This isn’t extremely exciting when no other three-dimensional transforms are in place, as there is nothing in particular to scale. In the demonstration below the elements are being scaled up and down on the z axis, however the rotateX value is added in order to see the behavior of the scaleZ value. When removing the rotateX in this case, the elements will appear to be unchanged.

3. 3D Translate
Elements may also be translated on the z axis using the translateZ value. A negative value here will push an element further away on the z axis, resulting in a smaller element. Using a positive value will pull an element closer on the z axis, resulting in a larger element.

While this may appear to be very similar to that of the two-dimensional transform scale value, it is actually quite different. The transform is taking place on the z axis, not the x or y axes. When working with three-dimensional transforms, being able to move an element on the z axis does have great benefits, like when building the cube below for example.4

4. 3D Skew:Skew is the one two-dimensional transform that cannot be transformed on a three-dimensional scale. Elements may be skewed on the x and y axis, then transformed three-dimensionally as wished, but they cannot be skewed on the z axis.



### Transitions & Animations:

-   *transition* to take place, an element must have a change in state, and different styles must be identified for each state. The easiest way for determining styles for different states is by using the :hover, :focus, :active, and :target pseudo-classes.
There are four transition related properties in total, including transition-property, transition-duration, transition-timing-function, and transition-delay. Not all of these are required to build a transition, with the first three are the most popular.
In the example below the box will change its background color over the course of 1 second in a linear fashion.

**Transitional Property**
The transition-property property determines exactly what properties will be altered in conjunction with the other transitional properties. By default, all of the properties within an element’s different states will be altered upon change. However, only the properties identified within the transition-property value will be affected by any transitions.

In the example above, the background property is identified in the transition-property value. Here the background property is the only property that will change over the duration of 1 second in a linear fashion. Any other properties included when changing an element’s state, but not included within the transition-property value, will not receive the transition behaviors as set by the transition-duration or transition-timing-function properties.

If multiple properties need to be transitioned they may be comma separated within the transition-property value. Additionally, the keyword value all may be used to transition all properties of an element.

**Transition Duration**
The duration in which a transition takes place is set using the transition-duration property. The value of this property can be set using general timing values, including seconds (s) and milliseconds (ms). These timing values may also come in fractional measurements, .2s for example.

**Transition** Timing
The transition-timing-function property is used to set the speed in which a transition will move. Knowing the duration from the transition-duration property a transition can have multiple speeds within a single duration. A few of the more popular keyword values for the transition-timing-function property include linear, ease-in, ease-out, and ease-in-out.

The linear keyword value identifies a transition moving in a constant speed from one state to another. The ease-in value identifies a transition that starts slowly and speeds up throughout the transition, while the ease-out value identifies a transition that starts quickly and slows down throughout the transition. The ease-in-out value identifies a transition that starts slowly, speeds up in the middle, then slows down again before ending.

* Animations
Transitions do a great job of building out visual interactions from one state to another, and are perfect for these kinds of single state changes. However, when more control is required, transitions need to have multiple states. In return, this is where animations pick up where transitions leave off.

**Animations Keyframes**
To set multiple points at which an element should undergo a transition, use the @keyframes rule. The @keyframes rule includes the animation name, any animation breakpoints, and the properties intended to be animated.

**Animation Name**
Once the keyframes for an animation have been declared they need to be assigned to an element. To do so, the animation-name property is used with the animation name, identified from the @keyframes rule, as the property value. The animation-name declaration is applied to the element in which the animation is to be applied to.


.stage:hover .ball {
  animation-name: slide;
}

* Customizing Animations:
1. Animation Iteration
2. animation direction
3. animation play state

### 8 SIMPLE CSS3 TRANSITIONS THAT WILL WOW YOUR USERS:
1. Fade in:Having things fade in is a fairly common request from clients. It’s a great way to emphasize functionality or draw attention to a call to action.

2. Change color:Animating a change of color used to be unbelievably complex, with all kinds of math involved in calculating separate RGB values and then recombining them. Now, we just set the div’s class to “color” and specify the color we want in our CSS

3. Grow & Shrink:To grow an element, you used to have to use its width and height, or its padding. But now we can use CSS3’s transform to enlarge.

4. Rotate elements: CSS transforms have a number of different uses, and one of the best is transforming the rotation of an element. Give your div the class “rotate” and add the following to your CSS

5. Square to circle: A really popular effect at the moment is transitioning a square element into a round one, and vice versa. With CSS, it’s a simple effect to achieve, we just transition the border-radius property.

6. 3D shadow
- 3D shadows were frowned upon for a year or so, because they weren’t seen as compatible with flat design, which is of course nonsense, they work fantastically well to give a user feedback on their interactions and work with flat, or fake 3D interfaces.

This effect is achieved by adding a box shadow, and then moving the element on the x axis using the transform and translate properties so that it appears to grow out of the screen.

7. Swing

- Not all elements use the transition property. We can also create highly complex animations using @keyframes, animation and animation-iteration.
In this case, we’ll first define a CSS animation in your styles. You’ll notice that due to implementation issues, we need to use @-webkit-keyframes as well as @keyframes (yes, Internet Explorer really is better than Chrome, in this respect at least).


8. Inset border
- One of the hottest button styles right now is the ghost button; a button with no background and a heavy border. We can of course add a border to an element simply, but that will change the element’s position. We could fix that problem using box sizing, but a far simpler solution is the transition in a border using an inset box shadow.

### read b:
- like most 25-year-olds, Julia Rozovsky wasn’t sure what she wanted to do with her life. She had worked at a consulting firm, but it wasn’t a good match. Then she became a researcher for two professors at Harvard, which was interesting but lonely. Maybe a big corporation would be a better fit. Or perhaps a fast-growing start-up. All she knew for certain was that she wanted to find a job that was more social. ‘‘I wanted to be part of a community, part of something people were building together,’’ she told me. She thought about various opportunities — Internet companies, a Ph.D. program — but nothing seemed exactly right. So in 2009, she chose the path that allowed her to put off making a decision: She applied to business schools and was accepted by the Yale School of Management.

When Rozovsky arrived on campus, she was assigned to a study group carefully engineered by the school to foster tight bonds. Study groups have become a rite of passage at M.B.A. programs, a way for students to practice working in teams and a reflection of the increasing demand for employees who can adroitly navigate group dynamics. A worker today might start the morning by collaborating with a team of engineers, then send emails to colleagues marketing a new brand, then jump on a conference call planning an entirely different product line, while also juggling team meetings with accounting and the party-planning committee. To prepare students for that complex world, business schools around the country have revised their curriculums to emphasize team-focused learning.

Every day, between classes or after dinner, Rozovsky and her four teammates gathered to discuss homework assignments, compare spreadsheets and strategize for exams. Everyone was smart and curious, and they had a lot in common: They had gone to similar colleges and had worked at analogous firms. These shared experiences, Rozovsky hoped, would make it easy for them to work well together. But it didn’t turn out that way. ‘‘There are lots of people who say some of their best business-school friends come from their study groups,’’ Rozovsky told me. ‘‘It wasn’t like that for me.’’

Instead, Rozovsky’s study group was a source of stress. ‘‘I always felt like I had to prove myself,’’ she said. The team’s dynamics could put her on edge. When the group met, teammates sometimes jockeyed for the leadership position or criticized one another’s ideas. There were conflicts over who was in charge and who got to represent the group in class. ‘‘People would try to show authority by speaking louder or talking over each other,’’ Rozovsky told me. ‘‘I always felt like I had to be careful not to make mistakes around them.’’

So Rozovsky started looking for other groups she could join. A classmate mentioned that some students were putting together teams for ‘‘case competitions,’’ contests in which participants proposed solutions to real-world business problems that were evaluated by judges, who awarded trophies and cash. The competitions were voluntary, but the work wasn’t all that different from what Rozovsky did with her study group: conducting lots of research and financial analyses, writing reports and giving presentations. The members of her case-competition team had a variety of professional experiences: Army officer, researcher at a think tank, director of a health-education nonprofit organization and consultant to a refugee program. Despite their disparate backgrounds, however, everyone clicked. They emailed one another dumb jokes and usually spent the first 10 minutes of each meeting chatting. When it came time to brainstorm, ‘‘we had lots of crazy ideas,’’ Rozovsky said.

One of her favorite competitions asked teams to come up with a new business to replace a student-run snack store on Yale’s campus. Rozovsky proposed a nap room and selling earplugs and eyeshades to make money. Someone else suggested filling the space with old video games. There were ideas about clothing swaps. Most of the proposals were impractical, but ‘‘we all felt like we could say anything to each other,’’ Rozovsky told me. ‘‘No one worried that the rest of the team was judging them.’’ Eventually, the team settled on a plan for a micro­gym with a handful of exercise classes and a few weight machines. They won the competition. (The micro­gym — with two stationary bicycles and three treadmills — still exists.)

Rozovsky’s study group dissolved in her second semester (it was up to the students whether they wanted to continue). Her case team, however, stuck together for the two years she was at Yale.

It always struck Rozovsky as odd that her experiences with the two groups were dissimilar. Each was composed of people who were bright and outgoing. When she talked one on one with members of her study group, the exchanges were friendly and warm. It was only when they gathered as a team that things became fraught. By contrast, her case-competition team was always fun and easygoing. In some ways, the team’s members got along better as a group than as individual friends.

*‘‘I couldn’t figure out why things had turned out so different,’’ Rozovsky told me. ‘‘It didn’t seem like it had to happen that way.’’*

ur data-saturated age enables us to examine our work habits and office quirks with a scrutiny that our cubicle-bound forebears could only dream of. Today, on corporate campuses and within university laboratories, psychologists, sociologists and statisticians are devoting themselves to studying everything from team composition to email patterns in order to figure out how to make employees into faster, better and more productive versions of themselves. ‘‘We’re living through a golden age of understanding personal productivity,’’ says Marshall Van Alstyne, a professor at Boston University who studies how people share information. ‘‘All of a sudden, we can pick apart the small choices that all of us make, decisions most of us don’t even notice, and figure out why some people are so much more effective than everyone else.’’

Yet many of today’s most valuable firms have come to realize that analyzing and improving individual workers ­— a practice known as ‘‘employee performance optimization’’ — isn’t enough. As commerce becomes increasingly global and complex, the bulk of modern work is more and more team-based. One study, published in The Harvard Business Review last month, found that ‘‘the time spent by managers and employees in collaborative activities has ballooned by 50 percent or more’’ over the last two decades and that, at many companies, more than three-quarters of an employee’s day is spent communicating with colleagues.

* In Silicon Valley, software engineers are encouraged to work together, in part because studies show that groups tend to innovate faster, see mistakes more quickly and find better solutions to problems. Studies also show that people working in teams tend to achieve better results and report higher job satisfaction. In a 2015 study, executives said that profitability increases when workers are persuaded to collaborate more. Within companies and conglomerates, as well as in government agencies and schools, teams are now the fundamental unit of organization. If a company wants to outstrip its competitors, it needs to influence not only how people work but also how they work together.

Five years ago, Google — one of the most public proselytizers of how studying workers can transform productivity — became focused on building the perfect team. In the last decade, the tech giant has spent untold millions of dollars measuring nearly every aspect of its employees’ lives. Google’s People Operations department has scrutinized everything from how frequently particular people eat together (the most productive employees tend to build larger networks by rotating dining companions) to which traits the best managers share (unsurprisingly, good communication and avoiding micromanaging is critical; more shocking, this was news to many Google managers).

The company’s top executives long believed that building the best teams meant combining the best people. They embraced other bits of conventional wisdom as well, like ‘‘It’s better to put introverts together,’’ said Abeer Dubey, a manager in Google’s People Analytics division, or ‘‘Teams are more effective when everyone is friends away from work.’’ But, Dubey went on, ‘‘it turned out no one had really studied which of those were true.’’

In 2012, the company embarked on an initiative — code-named Project Aristotle — to study hundreds of Google’s teams and figure out why some stumbled while others soared. Dubey, a leader of the project, gathered some of the company’s best statisticians, organizational psychologists, sociologists and engineers. He also needed researchers. Rozovsky, by then, had decided that what she wanted to do with her life was study people’s habits and tendencies. After graduating from Yale, she was hired by Google and was soon assigned to Project Aristotle.
- ject Aristotle’s researchers began by reviewing a half-century of academic studies looking at how teams worked. Were the best teams made up of people with similar interests? Or did it matter more whether everyone was motivated by the same kinds of rewards? Based on those studies, the researchers scrutinized the composition of groups inside Google: How often did teammates socialize outside the office? Did they have the same hobbies? Were their educational backgrounds similar? Was it better for all teammates to be outgoing or for all of them to be shy? They drew diagrams showing which teams had overlapping memberships and which groups had exceeded their departments’ goals. They studied how long teams stuck together and if gender balance seemed to have an impact on a team’s success.

No matter how researchers arranged the data, though, it was almost impossible to find patterns — or any evidence that the composition of a team made any difference. ‘‘We looked at 180 teams from all over the company,’’ Dubey said. ‘‘We had lots of data, but there was nothing showing that a mix of specific personality types or skills or backgrounds made any difference. The ‘who’ part of the equation didn’t seem to matter.’’

Some groups that were ranked among Google’s most effective teams, for instance, were composed of friends who socialized outside work. Others were made up of people who were basically strangers away from the conference room. Some groups sought strong managers. Others preferred a less hierarchical structure. Most confounding of all, two teams might have nearly identical makeups, with overlapping memberships, but radically different levels of effectiveness. ‘‘At Google, we’re good at finding patterns,’’ Dubey said. ‘‘There weren’t strong patterns here.’’

As they struggled to figure out what made a team successful, Rozovsky and her colleagues kept coming across research by psychologists and sociologists that focused on what are known as ‘‘group norms.’’ Norms are the traditions, behavioral standards and unwritten rules that govern how we function when we gather: One team may come to a consensus that avoiding disagreement is more valuable than debate; another team might develop a culture that encourages vigorous arguments and spurns groupthink. Norms can be unspoken or openly acknowledged, but their influence is often profound. Team members may behave in certain ways as individuals — they may chafe against authority or prefer working independently — but when they gather, the group’s norms typically override individual proclivities and encourage deference to the team.

Project Aristotle’s researchers began searching through the data they had collected, looking for norms. They looked for instances when team members described a particular behavior as an ‘‘unwritten rule’’ or when they explained certain things as part of the ‘‘team’s culture.’’ Some groups said that teammates interrupted one another constantly and that team leaders reinforced that behavior by interrupting others themselves. On other teams, leaders enforced conversational order, and when someone cut off a teammate, group members would politely ask everyone to wait his or her turn. Some teams celebrated birthdays and began each meeting with informal chitchat about weekend plans. Other groups got right to business and discouraged gossip. There were teams that contained outsize personalities who hewed to their group’s sedate norms, and others in which introverts came out of their shells as soon as meetings began.


- After looking at over a hundred groups for more than a year, Project Aristotle researchers concluded that understanding and influencing group norms were the keys to improving Google’s teams. But Rozovsky, now a lead researcher, needed to figure out which norms mattered most. Google’s research had identified dozens of behaviors that seemed important, except that sometimes the norms of one effective team contrasted sharply with those of another equally successful group. Was it better to let everyone speak as much as they wanted, or should strong leaders end meandering debates? Was it more effective for people to openly disagree with one another, or should conflicts be played down? The data didn’t offer clear verdicts. In fact, the data sometimes pointed in opposite directions. The only thing worse than not finding a pattern is finding too many of them. Which norms, Rozovsky and her colleagues wondered, were the ones that successful teams shared?

- magine you have been invited to join one of two groups.

Team A is composed of people who are all exceptionally smart and successful. When you watch a video of this group working, you see professionals who wait until a topic arises in which they are expert, and then they speak at length, explaining what the group ought to do. When someone makes a side comment, the speaker stops, reminds everyone of the agenda and pushes the meeting back on track. This team is efficient. There is no idle chitchat or long debates. The meeting ends as scheduled and disbands so everyone can get back to their desks.

Team B is different. It’s evenly divided between successful executives and middle managers with few professional accomplishments. Teammates jump in and out of discussions. People interject and complete one another’s thoughts. When a team member abruptly changes the topic, the rest of the group follows him off the agenda. At the end of the meeting, the meeting doesn’t actually end: Everyone sits around to gossip and talk about their lives.

Which group would you rather join?

In 2008, a group of psychologists from Carnegie Mellon, M.I.T. and Union College began to try to answer a question very much like this one. ‘‘Over the past century, psychologists made considerable progress in defining and systematically measuring intelligence in individuals,’’ the researchers wrote in the journal Science in 2010. ‘‘We have used the statistical approach they developed for individual intelligence to systematically measure the intelligence of groups.’’ Put differently, the researchers wanted to know if there is a collective I. Q. that emerges within a team that is distinct from the smarts of any single member.

To accomplish this, the researchers recruited 699 people, divided them into small groups and gave each a series of assignments that required different kinds of cooperation. One assignment, for instance, asked participants to brainstorm possible uses for a brick. Some teams came up with dozens of clever uses; others kept describing the same ideas in different words. Another had the groups plan a shopping trip and gave each teammate a different list of groceries. The only way to maximize the group’s score was for each person to sacrifice an item they really wanted for something the team needed. Some groups easily divvied up the buying; others couldn’t fill their shopping carts because no one was willing to compromise.

What interested the researchers most, however, was that teams that did well on one assignment usually did well on all the others. Conversely, teams that failed at one thing seemed to fail at everything. The researchers eventually concluded that what distinguished the ‘‘good’’ teams from the dysfunctional groups was how teammates treated one another. The right norms, in other words, could raise a group’s collective intelligence, whereas the wrong norms could hobble a team, even if, individually, all the members were exceptionally bright.

But what was confusing was that not all the good teams appeared to behave in the same ways. ‘‘Some teams had a bunch of smart people who figured out how to break up work evenly,’’ said Anita Woolley, the study’s lead author. ‘‘Other groups had pretty average members, but they came up with ways to take advantage of everyone’s relative strengths. Some groups had one strong leader. Others were more fluid, and everyone took a leadership role.’’

As the researchers studied the groups, however, they noticed two behaviors that all the good teams generally shared. First, on the good teams, members spoke in roughly the same proportion, a phenomenon the researchers referred to as ‘‘equality in distribution of conversational turn-taking.’’ On some teams, everyone spoke during each task; on others, leadership shifted among teammates from assignment to assignment. But in each case, by the end of the day, everyone had spoken roughly the same amount. ‘‘As long as everyone got a chance to talk, the team did well,*’’ Woolley said. ‘‘But if only one person or a small group spoke all the time, the collective intelligence declined.’’*

* Second, the good teams all had high ‘‘average social sensitivity’’ — a fancy way of saying they were skilled at intuiting how others felt based on their tone of voice, their expressions and other nonverbal cues. One of the easiest ways to gauge social sensitivity is to show someone photos of people’s eyes and ask him or her to describe what the people are thinking or feeling — an exam known as the Reading the Mind in the Eyes test. People on the more successful teams in Woolley’s experiment scored above average on the Reading the Mind in the Eyes test. They seemed to know when someone was feeling upset or left out. People on the ineffective teams, in contrast, scored below average. They seemed, as a group, to have less sensitivity toward their colleagues.

In other words, if you are given a choice between the serious-minded Team A or the free-flowing Team B, you should probably opt for Team B. Team A may be filled with smart people, all optimized for peak individual efficiency. But the group’s norms discourage equal speaking; there are few exchanges of the kind of personal information that lets teammates pick up on what people are feeling or leaving unsaid. There’s a good chance the members of Team A will continue to act like individuals once they come together, and there’s little to suggest that, as a group, they will become more collectively intelligent.

- n contrast, on Team B, people may speak over one another, go on tangents and socialize instead of remaining focused on the agenda. The team may seem inefficient to a casual observer. But all the team members speak as much as they need to. They are sensitive to one another’s moods and share personal stories and emotions. While Team B might not contain as many individual stars, the sum will be greater than its parts.

Within psychology, researchers sometimes colloquially refer to traits like ‘‘conversational turn-taking’’ and ‘‘average social sensitivity’’ as aspects of what’s known as psychological safety — a group culture that the Harvard Business School professor Amy Edmondson defines as a ‘‘shared belief held by members of a team that the team is safe for interpersonal risk-taking.’’ Psychological safety is ‘‘a sense of confidence that the team will not embarrass, reject or punish someone for speaking up,’’ Edmondson wrote in a study published in 1999. ‘‘It describes a team climate characterized by interpersonal trust and mutual respect in which people are comfortable being themselves.’’

When Rozovsky and her Google colleagues encountered the concept of psychological safety in academic papers, it was as if everything suddenly fell into place. One engineer, for instance, had told researchers that his team leader was ‘‘direct and straightforward, which creates a safe space for you to take risks.’’ That team, researchers estimated, was among Google’s accomplished groups. By contrast, another engineer had told the researchers that his ‘‘team leader has poor emotional control.’’ He added: ‘‘He panics over small issues and keeps trying to grab control. I would hate to be driving with him being in the passenger seat, because he would keep trying to grab the steering wheel and crash the car.’’ That team, researchers presumed, did not perform well.

Most of all, employees had talked about how various teams felt. ‘‘And that made a lot of sense to me, maybe because of my experiences at Yale,’’ Rozovsky said. ‘‘I’d been on some teams that left me feeling totally exhausted and others where I got so much energy from the group.’’ Rozovsky’s study group at Yale was draining because the norms — the fights over leadership, the tendency to critique — put her on guard. Whereas the norms of her case-competition team — enthusiasm for one another’s ideas, joking around and having fun — allowed everyone to feel relaxed and energized.