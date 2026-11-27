# Persistent Memory

When I open a new chat and say “let’s pick up where we left off,” I want it to know what we finished, what I corrected, and what still needs doing. I direct the project and set the tests. AI coding assistants help me build and evaluate the prototype. The question I use to judge it is simple. What answer does the person actually get before they have to explain themselves again?

## 2024–2025 · Why I started

**February 22 and 27, 2024 · The first dated requests I found.** On February 22, I asked Gemini whether it could keep one personal detail on my phone so it would have it next time. Five days later, I asked whether it could use my storage to keep things we discussed. I wanted to come back to ideas I might otherwise forget. Those conversations date the idea. The exact day I began building the software is still unknown.

**July 18 and 20, 2024 · Who chooses what the assistant remembers?** I proposed letting the user choose which information an assistant could access. Two days later I ran into a practical example. I was trying to give the assistant my résumé so it would understand my background, and I couldn’t get it into the conversation.

**December 16, 2024, and January 8–11, 2025 · Why the résumé mattered.** In December I asked whether Gemini could save what I was about to tell it, then described my progression through IT and systems administration. On January 8 I explained the consequence of starting from scratch. Without that background, I had to explain my experience before we could get to the actual question. On January 11 I explicitly raised having to upload the résumé repeatedly. That gave the project a concrete requirement a user could recognize.

**September 16, 2025 · The right keywords were too much to ask of the user.** While discussing project files and photographs, I described having to supply keywords to bring back an earlier discussion. That experience shaped how I test today. A person who has forgotten the details is precisely the person who can’t supply the perfect search phrase.

## 2026 · From personal workflow to prototype

**February 10–11 · Putting context somewhere the assistant could find it.** I organized a folder about my computer build and projects. The next day I clarified that I wanted the assistant to find the information itself. Explaining another screenshot still left me doing the remembering.

**May 26 · A local build was already underway.** The earliest Codex project conversation I could verify opens with me asking it to inspect the Jarvis and Atlas memory setup I already had. By this date there was something on my computer to inspect. The record starts partway through the work.

**June 2 and July 20 · Access and recall turned out to be separate problems.** In June I checked which folders the assistant could actually reach. In July I was troubleshooting why a new session still lost context. Opening a file on request answered one question. The harder one was whether a new chat would recognize which file or conversation mattered without directions from me.

**August 22 · Rules for keeping originals and corrections.** I set limits on which original messages and reviewed images could be saved. A later correction needed to stay connected to the earlier statement while preserving what had originally been said. That mattered when we began grading answers against changed plans.

**September 13 · First substantial evaluation documented here.** A study with 24 fictional situations produced 48 saved assessments. All 48 requests completed, yet the software initially couldn’t read 14 responses. After a repair we could read all 48 on replay. Of those, 47 passed the checks tying the evidence back to its sources. One was withheld. Even among the readable responses, some still drew the wrong conclusion. That gave us a reason to score recovery and interpretation separately.

**October 7 · Testing the choice of earlier evidence.** A revised version passed 193 component tests and 13 staged checks. We also replayed two earlier questions to check which sources it selected. We could verify the revision was registered on the computer. We still needed to observe it helping someone in a real conversation.

**October 8 and 22 · Keeping my place between projects.** I kept putting related work in different chats and then losing track of it. On October 8 I asked for a way to come back to a project. We organized the recovered work into 20 project homes and checked that 1,340 original files still had the same contents. On October 22 I asked about finding an older conversation by its ID. These were tools I could use to find my place. I still wanted a new chat to recognize the subject when I didn’t know the ID.

## November 2026 · What happened in actual chats and controlled tests

**November 3 · One link, three conversations.** I pasted the same link into three different conversations within four minutes. The first two couldn’t read the post. In the third, I supplied only the URL. Before I mentioned the other attempts, the assistant recognized both failures, asked for browser access, and reviewed the post after I approved. On November 6 we checked the original messages and actions. The third conversation had already existed for several days. This was the clearest real example of the behavior I wanted, and it raised a question we could test. Would the same thing happen in a brand-new chat?

**November 9 · Resuming a project with an ordinary question.** After we updated the project guides, I asked a new web chat outside the project what we had finished and what came next. Its first answer recovered the latest engineering result, the limits of the test and the correct unfinished work. It cited the updated guides. The chat could also draw on earlier context, so several sources may have contributed. We tried the same question in a fresh Work chat. It cited an older review and missed part of the progress. Before the guide update, both answers had been incomplete.

**November 9 · Could I undo an update on my own computer?** We applied a revision to the Windows installation, restored the original file, and checked that its contents matched the original exactly. We then applied the revision again and verified which version was in place. That gave me a tested way back if the update went wrong. We tested what a new chat could remember separately.

**November 11 · Comparing the same link in fresh Codex chats.** Each chat received the same URL with no explanation, using the same model and browsing restrictions. The project chat recognized the two earlier failures. The comparison chat with standard Codex memory asked for the post text or a screenshot and gave no indication it recognized them. A third chat outside the project received the earlier records and still didn’t mention them. This isolated a real difference in those answers. One link couldn’t establish which part of the setup caused it or how often it would work elsewhere.

**November 12–13 · Did a chat find my correction, or did a summary give it the answer?** We checked two different corrections. On November 12, a new desktop chat found my original explanation of what I wanted a business idea to fund. It later saw a recap before answering, so we could verify how it found the original, but the recap could also have influenced the reply. In a separate, constrained fresh Codex run, I asked which app I had used for the three link attempts. The answer correctly said all three took place in Codex and cited my correction. We found no answer-giving summary in that run’s inputs. An ordinary desktop follow-up reached material that gave away the answer and was stopped before a final reply. Everyday desktop recovery remains an open question.

**November 14 · A work queue for the person managing the projects.** A local queue brought 16 tracked items into one view alongside an inventory of 24 projects. I could see ownership, what was waiting and where to pick up. It gave me a way to resume work even on days when a chat missed the handoff.

**November 19 · What did one attempt actually cost?** We recorded how many tokens an assistant and its helper processed during a link review, including how much input they reused. The account meter showed the same whole percentage before and after. The assistant could count the work it did, but it still couldn’t open the clip. We couldn’t assign an exact fraction of the weekly allowance to that attempt. I wanted to track whether a job finished alongside how much it used.

**November 20 · A changed location and an unaccepted suggestion.** In a fresh fictional test, one pickup moved while a second pickup stayed as arranged. The assistant applied the move to the right event and correctly treated a proposed time as a suggestion. It also added “AM” where the records gave no time of day. Someone following the answer would have received one detail too many.

**November 21 · Could a correction survive an interruption?** On one Windows PC we interrupted the prototype at four different points while it was saving. After restarting, all four cases recovered a weaving lesson moved from 9:15 a.m. to 2:50 p.m. and preserved a separate clarinet lesson at 11:40 a.m. In a fifth case, the saved records conflicted and the reader withheld both times. Physical power loss remains untested.

**November 21 · Could the first answer find the right topic?** In a separate Windows browser test, the prototype searched across 26 fictional topics and fully answered 19 of 20 previously exercised questions. On the twentieth, it asked which project I meant. The available conversation already said to bring four printed copies of a poem. Asking me again was the failure we were trying to catch. When we gave the revised reader the right original messages up front, it fully answered all 20 on replay. In everyday use, the assistant has to both find the right conversation and read it correctly.

**November 21 · What the phone test showed.** The Android browser displayed 40 answers generated by the model on my Windows PC. That verified delivery to the phone. A new conversation in the ordinary Android app still needed its own first-answer test.

**November 22 · Who took over the folding stools?** A repair got eight previously missed handoff examples right on replay. We then asked two fresh test chats the same question about a new fictional outing. Each found the intended conversation.

- **With the complete conversation**, Nell explicitly agreed to take the folding stools from Mavis. The assistant quoted Nell accepting the job, then told the reader it couldn’t verify that anyone had taken over. The answer should have named Nell.
- **With Nell’s final confirmation removed**, Mavis was the last documented person responsible for the stools. The assistant reasonably left the transfer open. Its answer missed a separate duty that was confirmed in the remaining conversation. Nell had agreed to take the direction cards. A useful answer could say exactly what was settled and what was still uncertain.

**November 23–24 · Moving updates between assistants and checking who said what.** On November 23, two assistants correctly read back an updated background record when prompted. Automatic sharing between them remains unverified. On November 24, a proposed change identified the speaker correctly in four of six small checks. It mistook a heading for a person in one and attributed someone’s quoted words to the wrong speaker in another. The change remains under evaluation.

**November 25 · Seeing who picked up the work.** In the desktop chat, I can now ask which tracked items need another look and see why. In one check, two of 16 items pointed to records that had changed. In another, the view showed that both assistants had acknowledged an earlier update. A third check showed why a saved answer needed a second opinion. The assistants had been prompted for the original handoff. Today’s checks ran locally, and a new advisor response is still untested.

**November 25 · Finding a project in a few words.** I compared two versions of the lookup on the same Windows computer. I tried seven short phrases I use for ongoing work. The earlier version found the intended note for none of the seven. The updated version found it for all seven. When one name fit two discussions, it showed both choices. This tested which note the computer could find. I still need to see whether a new desktop chat uses that note correctly in its first answer.

**November 25 · A source link can lead straight past the correction.** In a fictional case about who was handling the red lanterns, the lookup returned the earlier plan and a link to the conversation. The later correction was there when we opened the original. It was missing from the lookup result. This check ended before a model answered. That distinction matters to me because a relevant link alone still leaves the user to do the remembering.

**November 26 · When the assistant asks for confirmation, does it wait?** We ran eight short episodes in a computer simulation with two boxes. The local model passed six. In one of the other two it asked for confirmation in words while moving the orange box. After the operator clarified which box they meant, both boxes ended up in the delivery bay. In the other episode the simulator couldn’t interpret the model’s chosen actions. Seeing the words and the moves side by side gave us a way to catch a failure we’d miss by grading the conversation alone.

**November 26 · Trying the correction again with a hold in place.** In the next simulation, the test specified when a box had to stay put and when the operator had released it. Across six new two-step episodes, the boxes ended up in the correct positions after all 12 steps. The model chose the expected action on 11. On the remaining step it tried to move early and the simulator prevented it. This tells me the hold worked when the test supplied it. Whether the system can recognize that instruction in ordinary speech is still open.

**November 26 · Measuring work across open chats.** I wanted a record I could check when several chats were running at once. In one completed research turn, we reconciled its token counts across 21 updates and checked the account meter around the same work. Other chats overlapped. I could see how much text this turn processed and which part was cached, but couldn’t assign the later change in the shared allowance to this turn alone.

## What I’m working toward

A new chat should be able to answer “who’s taking care of that now?” from the latest agreement. If it has only the request to take over, it should name the last confirmed owner and explain what’s missing. I want that to work on an unfamiliar example, on the first reply, without my supplying an old conversation or a summary that gives away the answer.

Updated November 26, 2026.
