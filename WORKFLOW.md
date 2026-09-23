1. Walk through the final calculateLateFee function and name which contributor's change is responsible for each part.



The final calculateLateFee function follows four rules. If a loan is one day late or less then there is no fee. The fee calculation uses Math.round(). The result is capped at a minimum of $1 and a maximum of $20. Clone A supplied the grace period Clone B supplied the rounding Clone C supplied the fee cap and Clone A also supplied the minimum fee during the rebase.



2\. Compare Task 3's two-way conflict to Task 5's three-way conflict — what got harder with a third line of work?



The conflict in Task 3 was a two‑way conflict, it happened between the grace period change and the rounding change. In Task 5 a three‑way conflict appeared, Clone C added the fee cap so there were three contributors and the three‑way merge had to keep all three changes.



3\. What's the actual difference between how you resolved Task 5 (merge) and Task 6 (rebase)?



I used merge to combine changes into a merge commit in Task 5 and used rebase to place my minimum fee commit on top of the remote changes and rebase created a history and avoided the need for a force push in task 6.



4\. If this were a real team of three, what one process change would have prevented all three rejected pushes?



If it were a real team of three, the process of updating would have reduce the rejected pushes and avoid conflicts from outdated branches.





Screenshot Evidence:



!\[Task 1 Screenshot](screenshots/task-1.png)



!\[Task 2 Screenshot](screenshots/task-2.png)



!\[Task 3 Screenshot](screenshots/task-3.png)



!\[Task 4 Screenshot](screenshots/task-4.png)



!\[Task 5 Screenshot](screenshots/task-5.png)



!\[Task 6 Screenshot](screenshots/task-6.png)



!\[Task 7 Screenshot](screenshots/task-7.png)

