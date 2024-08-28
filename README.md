# For Rent Unjustified Eviction Fix

The game states that if a tenant breaks a rule, is overdue on rent,
or is within the grace period, eviction is justified. The label on
the eviction button will be "Justly Evict". However, EA wrote the
test for applying penalties in the case of unjustified eviction
incorrectly: a tenant can break the rules and be overdue on rent,
but as long as they're not also in the grace period, the game
will act as if the eviction was unjustified. Any one of those
conditions not being met will trigger the bug.

This mod adjusts the tests to ensure that the conditions are
checked properly, and the game will only consider an eviction
unjust with none of them met.

Bug Report: [[NEEDS SAVES] [FR] Justly evicting and still being fined](https://answers.ea.com/t5/Bug-Reports/NEEDS-SAVES-FR-Justly-evicting-and-still-being-fined/td-p/13289586)
