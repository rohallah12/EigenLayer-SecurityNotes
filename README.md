## This repository contains issues discovered in projects integrated with EigenLayer

<b>Project:</b> KelpDao <br>
<b>Author:</b> MixBytes <br>
<b>Issue:</b> When removing a nodeDelegator (a component of the system which deposits its ETH balance into EigenLayer) ETH balance of the contract must be equal to 0 <br>
<b>Link:</b> https://solodit.xyz/issues/lack-of-verification-for-the-native-eth-balance-and-staking-balance-in-the-eigenpod-mixbytes-none-kelpdao-markdown <br>

<hr>

<b>Project:</b> RioNetwork <br>
<b>Author:</b> Sherlock <br>
<b>Issue:</b> When depositing funds into EigenLayer, round down/ups when converting assset<=>shares must be taken into account. <br>
<b>Link:</b> https://solodit.xyz/issues/m-1-depositing-to-eigenlayer-can-revert-due-to-round-downs-in-converting-shares-assets-sherlock-rio-network-git <br>

<hr>

<b>Project:</b> EigenLayer <br>
<b>Author:</b> Code4Arena <br>
<b>Issue:</b> Lack of validation for length of provided proof. the `computedHash` of the proof was set to `leaf` initialy (before entering the `for-loop`), which means that
if length of `proof` is zero, the `for-loop` will not be entered and `computedHash` will be equal to `leaf` which will bypass the condition `require(leaf==proof)`<br>
<b>Link:</b> https://solodit.xyz/issues/h-01-slot-and-block-number-proofs-not-required-for-verification-of-withdrawal-multiple-withdrawals-possible-code4rena-eigenlayer-eigenlayer-contest-git <br>
