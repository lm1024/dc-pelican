title: Three Times Done
date: 2015/01/11

<p>In my experience many organisations experience systemic difficulties in getting work 'done' to an acceptable standard. The Scrum solution for this is 'agreed definition of done', which typically leads to a checklist eg</p>
<ul>
<li>the work has been checked in to the VCS</li>
<li>it builds ok</li>
<li>the automated tests pass</li>
<li>documentation exists, etc.</li>
</ul>
<p>That's great, assuming that infrastructure to satisfy the checklist actually exists and is stable. Often on projects we find ourselves having to create the infrastructure itself, and define/agree workable procedures relative to the specific work we need to do.</p>
<p>And in an R&amp;D or services environment with lots of variance in project parameters (scale, technology, risks, scope, terms) we often struggle to nail down what 'done' actually means. </p>
<p>In many cases, 'done' on a single project needs to mean different things at different times and for different types of work.</p>
<p>For example, a thorough and formal 'done' with tests and documentation etc may be great for ensuring a satisfactory delivery, but it would impede prototyping to establish whether the project is feasible in the first place.</p>
<p>So I'm proposing that we can explicitly consider software work in three modes:</p>
<ul>
<li>R&amp;D</li>
<li>ENGINEERING</li>
<li>PRODUCTION </li>
</ul>
<h3>1: R&amp;D</h3>
<p>(Feasibility, prototype, proof of concept, demo, hack, kludge, experiment, investigation, research)</p>
<p>At this stage we want to get to a specific result, but don't really care how we get there. The emphasis is on</p>
<ul>
<li>gaining information - can it be done? how should it be done?</li>
<li>reducing risks</li>
<li>providing proof, a demonstration, a video, a report</li>
<li>collecting and documenting ideas, opportunities, obstacles, risks to help in later stages</li>
<li>getting to the end as fast as is reasonably possible</li>
</ul>
<p>Crucial thing to note here is that by default this type of work should typically happen in a fast, creative, cut-as-many-corners-as-we-can-to-get-there style.</p>
<p>Any systems/solutions/software that we spin up for this should normally be considered to be throw-away or temporary. If a stated objective is to <em>use</em> the output in some way, that use should be noted as risky, experimental etc, since it will exploit piece of work which is ill-defined and will be of uncertain quality. </p>
<p>The two key traps to avoid are</p>
<p>A) management thinking that the resulting demo/POC actually does anything that can be used/sold/delivered.
B) engineers fearing that management will want to deliver the result</p>
<p>Trap A) leads to stressed engineers, and users receiving systems with fundamental design/approach flaws
Trap B) leads to engineers wasting time and effort on things which ultimately are not required</p>
<h3>2: ENGINEERING</h3>
<p>(Engineered, developed, coded, tested, reviewed, signed off)</p>
<p>Now we want to implement something for real. The result of this will be used by other people, so it needs to be designed properly, perform fast enough, be reliable, deal with bad user inputs etc. The output from this is expected to be some system/solution/software that the engineers believe is 'done'. </p>
<p>It does the job.</p>
<p>The key trap here is</p>
<p>C) Management thinking that the resulting engineering solution is the end of the project. In most cases, a range of follow-on activities will be required after engineering is notionally 'complete' to get the result adopted and running for its target users. The gap may include data migration, deployment, releasing, training, soak testing, backups, user setup, security, maintenance planning etc.</p>
<p>Even exceptional engineers will not have time or mental bandwidth to do these necessary things while designing and coding the solution itself.</p>
<p>However we must ensure that the engineering output from this phase includes all of the notes, ideas, limitations and documentation that the team have generated getting this far, as input into what comes next...</p>
<h3>3: PRODUCTION</h3>
<p>(Live, in production, integrated, released, delivered, published, deployed, documented, released, validated, accepted, upstreamed, in mainline, being maintained)</p>
<p>This phase is where the real world kicks in. All of the assumptions and knowledge gaps that were implicitly influencing the engineers working in phase 2) are now exposed as other people try to take the result and roll it into production, get it through acceptance, sign it off, use it for real etc.</p>
<p>Traps here include</p>
<p>D) expecting the engineers that did phase 2) to deal with phase 3) - it's unlikely that they'll be effective at exposing their own blind spots and assumptions.
E) assuming that this phase will take less effort than the one before it</p>
<h3>Notes</h3>
<ul>
<li>We are not assuming that all pieces of work go through all phases</li>
<li>When working on R&amp;D or ENGINEERING we still need to consider that PRODUCTION may/will happen later, and ensure the results of that thinking are recorded and passed on in an effective way.</li>
<li>It will not always be possible to separate the work this way - however explicitly clarifying which phase an activity fits into should help to establish what needs doing, and how the job should be approached.</li>
</ul>
<p>Finally, note that work done when we focus on real delivery may expose deep misunderstandings and/or issues which invalidate much or all of the previous effort. So remember "Code less. Every line creates a work chain. Code is a liability, not an asset"</p>
