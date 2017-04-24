# Stopping Rules

Some ideas or rules on when we might stop testing.

1. Time has run out. This, for many testers, is the most common one: we stop testing when the time allocated for testing has expired.

2. The Piñata Heuristic. We stop whacking the program when the candy starts falling out—we stop the test when we see the first sufficiently dramatic problem. (Bolton)

3. The Dead Horse Heuristic. The program is too buggy to make further testing worthwhile. We know that things are going to be modified so much that any more testing will be invalidated by the changes. (Bolton)

4. Mission is accomplished. We stop testing when we have answered all of the questions that we set out to answer.

5. Mission has been revoked.

6. The I Feel Stuck! Heuristic. For whatever reason, we stop because we perceive there’s something blocking us. We don’t have the information we need (many people claim that they can’t test without sufficient specifications, for example). There’s a blocking bug, such that we can’t get to the area of the product that we want to test; we don’t have the equipment or tools we need; we don’t have the expertise on the team to perform some kind of specialized test. (Bolton)

7. The Pause That Refreshes Heuristic. Instead of stopping testing, we suspend it for a while. We might stop testing and take a break when we’re tired, or bored, or uninspired to test. We might pause to do some research, to do some planning, to reflect on what we’ve done so far, the better to figure out what to do next. The idea here is that we need a break of some kind, and can return to the product later with fresh eyes or fresh minds.
There’s another kind of pause, too: We might stop testing some feature because another has higher priority for the moment.(Bolton)

8. The Flatline Heuristic. No matter what we do, we’re getting the same result. This can happen when the program has crashed or has become unresponsive in some way, but we might get flatline results when the program is especially stable, too—”looks good to me!” (Bolton)

9. The Customary Conclusion Heuristic. We stop testing when we usually stop testing. There’s a protocol in place for a certain number of test ideas, or test cases, or test cycles or variation, such that there’s a certain amount of testing work that we do, and we stop when that’s done. Agile teams (say that they) often implement this approach: “When all the acceptance tests pass, then we know we’re ready to ship.” Ewald Roodenrijs gives an example of this heuristic in his blog post titled When Does Testing Stop? He says he stops “when a certain amount of test cycles has been executed including the regression test”.
This differs from “Time’s Up”, in that the time dimension might be more elastic than some other dimension. Since many projects seem to be dominated by the schedule, it took a while for James and me to realize that this one is in fact very common. We sometimes hear “one test per requirement” or “one positive test and one negative test per requirement” as a convention for establishing good-enough testing. (We don’t agree with it, of course, but we hear about it.) (Bolton)

10.  No more interesting questions. At this point, we’ve decided that no questions have answers sufficiently valuable to justify the cost of continuing to test, so we’re done. This heuristic tends to inform the others, in the sense that if a question or a risk is sufficiently compelling, we’ll continue to test rather than stopping. (Bolton)

11. The Avoidance/Indifference Heuristic. Sometimes people don’t care about more information, or don’t want to know what’s going on the in the program. The application under test might be a first cut that we know will be replaced soon. Some people decide to stop testing because they’re lazy, malicious, or unmotivated. Sometimes the business reasons for releasing are so compelling that no problem that we can imagine would stop shipment, so no new test result would matter. (Bolton)

12. Mission Rejected. We stop testing when we perceive a problem for some person—in particular, an ethical issue—that prevents us from continuing work on a given test, test cycle, or development project. (Bolton, Kaner)

## Credits

* Most of these rules come from Michael Bolton's article [When Do We Stop Testing?](http://www.developsense.com/blog/2009/09/when-do-we-stop-test/)_
