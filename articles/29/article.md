#Lecture Notes, Issue 33

{'Author': 'The Librarian Staff', 'Date': '9.10.17', 'Category': 'Review', 'Tags': ('History', 'Physics', 'Radio', 'Stipatores Honorati', 'Lectures'), "Issue": "Supplementary Issue 1"}

Many lectures are delivered by a single person or group of people. It
would soon become tedious for both the writer and the reader to
continually write “$x$ claims/says/posits that $y$”. We shall therefore
in most cases only include $y$, ie. what is said.

To aid clarity, articles here are split into two sections. The first is
in normal font, and describes what was said. The second is in **bold**,
and is commentary. Commentary is occasional or sometimes non-existent.
The former, ie. an account of what happened, will be as objective as
possible, such that even if a completely false claim is made, it is
still repeated eg. “Paris is the capital of Germany”. Commentary may
point out false claims - “**Paris is actually the capital of France.
Germany’s capital is Berlin**”. This two part structure will hopefully
maximise clarity.

Stipatores Honorati
-------------------

Last month, the inaugural meeting was held up Refectory of Stipatores
Honorati, which translates as the Following of St. Honoré (the patron
saint of bakers, among other things including candle-makers, florists,
flour merchants, corn chandlers, and oil refiners, who, as those
attending were told, resisted his election as bishop of Amiens,
believing himself unworthy of the post, but nevertheless found himself
the target of a ray of divine light upon his election, the news of which
his nursemaid, baking bread at the time, refused to believe unless the
peel (a shovel-like object) she was using at the time put down roots and
became a tree, which it, somewhat predictably for such stories, did, in
the form of a mulberry tree), more informally known as Cake Society, at
which, each month, a speaker brings and shares a cake and some
information on its history and literary references, in this case a
Northamptonshire Seblet Cake (a seed cake made with caraway) provided by
William Mirza, who set up and runs this society (with supervision from
the Chaplain), and who spoke of the various references to it and seed
cakes like it in such books as Jane Eyre and the Hobbit, before opening
the society up to general discussion of such issues as the pronunciation
of scone (all but one agreed it rhymed with gone), whether one puts jam
or clotted cream onto said scone first (all but one put cream on first,
raising such reasons as the fact that clotted cream is more solid than
good jam, thus making it easier to get an even spread with cream first,
and the way clotted cream can fulfill the functions of butter on the
scone (although it was noted that some get around this by using butter
as well, in a show of extreme overindulgence)), why poppy seeds were so
popular in cakes these days, whether Britain had ever successfully
invaded Afghanistan, whether Stipatores Honorati was an acceptable name
(which thankfully it was, as a dedicated cake slice had already been
engraved), and which cakes should be the subject of upcoming meetings,
with the final decision that, as Stipatores Honorati is set to be
monthly, October would have William Mirza speaking on Oxford Apple Buns,
owing to it being apple season, November would have Adam Mee on Colin
the Caterpillar, a famous Marks and Spencer chocolate roll cake,
December would have something Christmas related, and January would have
this author on Black Bun, a Scottish delicacy eaten at Hogmanay. It was
enjoyed by all.

Wireless Circuits in the Age of the Internet of Things
------------------------------------------------------

This lecture was delivered by Professor Alyssa Apsel, of Cornell
University. She works in the field of low power radio.

Professor Apsel first explained her thoughts on engineering - to her, it
is a combination of creativity and numeracy, hence her interest.

Radio is used for all sorts of information, not just “radio”. It
includes electromagnetic waves where $3\text{kHz} < f < 300\text{GHz}$.
The transmission of data occurs by the modulation of frequency, phase
and amplitude. Amplifiers amplify signals which are broadcast by
antennae. Most reception is small and noisy. Demodulation is the process
of getting information from this reception. One can filter signal by the
size of one of the modulated things.

Low power radio is P2P, has low bitrate and complexity, and can describe
a single usage case of a broader system. Power consumption is below
$100$mW.

Power is useful in that it increases range and resilience, amongst other
things. By extension, low power radios must adapt in order by either
minimising range and resilience or reducing the factors which cause this
phenomenon.

There are three basic architectures of radio. The first is narrow band.
It has high penetration and resilience, and there are many variants. The
second is UWB - ultra wideband. Short transmissions with high bitrate
are sent over short to medium distances. The final type is passive -
this includes NFC and RFID.

Narrow band encodes bit streams by the use of a number of processes,
such as BPSK, OOK and FSK. Complex multi-value phase transmissions allow
more data to be sent - instead of a binary transmission, transmissions
may allow more than one value per bit. The baseband - the original
frequency of the data - is likely to be low. The data are converted to
high frequency by a modulator and oscillator. The receiver’s demodulator
will reverse this process.

Amplifiers are used to increase signal strength. Low noise amplifiers
must be specific to frequencies in order to minimise distortion. They
use lots of power, since a decrease in power increases noise.
Transmitters, again, are also power-hungry. In short, power usage is
dominated in transmitters by the oscillator and the amplifier, and in
receivers by the oscillator and low noise amplifier.

There is therefore a necessary trade-off between low power usage and
other desiderata, such as bitrate and range. Hence low power radios must
be low range, low bitrate and have low overhead. Alternatively, they may
have high off time, or be asymmetric.

A question from the audience asked how other frequencies were
eliminated. Some inductors and capacitors have a specific resonance, so
only one frequency will get through. At other times, a fast signal is
slowed down, and their difference subtracted, in order to get the
original signal.

The internet of things refers to the expansion of the internet to
everyday objects, such as fridges and lightbulbs. This permits seemless
automation. However, low power and cost is required given the number and
cost requirements of these items. Existing infrastructure is
insufficient, both in power and capacity terms.

Low power protocols include Zigbee, Bluetooth LE, ANt and WiFi Halo.

Khanh Tuan Le’s paper “Designing a ZigBee-ready IEE 802.15.4-compliant
radio tranceiver” provides some more useful information.

**This is available at
<https://citeseerx.ist.psu.edu/Khan/download?doi=10.1.1.214.3734&rep=rep1&type=pdf>**

Other ways of reducing power usage include wideband, which does not
require modulators on the other side, and passive systems. Asymmetric
systems are used where power is available in abundance on one side, and
to a much lesser degree on another - an example is cellular data.
Passive radio takes this to the extreme. The power of the receiver or
transmitter is so great that the other side needs very little or no
power. This works because if, for example, a cellular tower has a very
powerful antenna, a phone does not require a very good amplifier (or a
very high power amplifier) to receive this signal accurately and
quickly.

Finally, Apsel spoke of some of her research. For radios which save
power by switching off, there is a need for some sort of synchronisation
or other mechanism to ensure that radios are on at the same time.
Synchronisation of clocks in many different places is very difficult.

Her research explored the possibility of using a similar mechanism to
fireflies in South East Asia. Using distributed synchronisation,
fireflies, or receivers, adapt to the fastest cycle. Gradually, they
synchronise by themselves. Her team managed to ensure four nodes
synchronised.

There is, however, a lacuna in authentication in this method. An
malicious actor could use a very fast transmitter, or firefly, in order
to sabotage the cycle.

**Given this is merely research and implementation is a long way away,
this is not particularly problematic. Obviously some sort of
authentication would be required in order to prevent sabotage were it to
be used widely.**

What’s the wrong thing to do?
-----------------------------

Dr. Rufus Duits in this lecture proposed four premises to this argument,
and one conclusion.

1.  Reasons internalism says that reasons for action must come from
    within the self and cannot be implanted. An example is that though
    another may urge me to drink poison, I do not wish to drink poison,
    and so I have no reason to do so. Reasons externalism is the
    opposite view.

    **This is somewhat plausible - note that external actors’ urgings
    may still have value if one internally wishes to please others.**

2.  Reasons instrumentalism says that practical reasoning is exclusively
    about means or intermediate ends as means. If there are two motives
    $x$ and $y$ such that there is no common motive z for which x
    and y are intermediate motives, there is no way to decide between
    x and y.

3.  Moral rationalism says that morally wrong actions must have an
    overriding reason for their not being done.

4.  A distinction is morally relevant if it is not said to be so *ex
    post facto*, and is universalisable. Moral impartialism holds that
    where two situations are relevantly similar, that which is morally
    correct to do is the same.

Given this, one must not do $x$ where $x$ affects another party such
that they have an overriding reason to object based on a principle.

**The derivation of this last claim is somewhat tenuous - in the
lecture, due to time constraints, by no fault of Dr. Duits, it was
nearly nonexistent. We shall attempt to reconstruct the derivation.**

**By (2), it is unclear which of two parties in a moral dispute is
correct, given that reasons for action must come from within the self.
By (4), there is no morally relevant distinction between the other
person and me, and so our internal motivations are equally important,
and so by (1) we should value their own internal reasoning, hence the
claim.**

Dr. Duits says that if we accept all four claims we must necessarily
accept his fifth.

**It is also worth noting that an objection based on the absurdity of
universalisability does not stand, insofar as such objections generally
assert that there is difficulty in determining good faith when
classifying actions. However, given that all that is required, at least
for this interpretation of the argument, is that there be no morally
relevant distinction between people, universalisability criteria may
break down elsewhere without causing this argument to fail.**

The Gladstone Problem
---------------------

Emeritus Professor Michael Bentley’s talk is about both Gladstone and
historiographic problems encountered in his study.

Gladstone is “something vaguely colossal”: he crosses the century. This
less to problems in analysis. He was alive from 1809 to 1898, in the
Commons from 1830 to 1894 and in the cabinet from 1843.

Gladstone’s energy lead to what would now likely be diagnosed as OCD. He
had to chew all his food 36 times. One diary entry wrote that he had
“bathed 17 times” in a morning. Yet he was also extraordinary - in one
morning he also wrote “41 letters” according to that same diary. There
are historiographic problems as a result of this, for he is so large,
and extraordinary, that we feel somewhat overawed and guilty in
criticising him.

Gladstone was not orginally meant to take the liberal direction he did.
Compare Peel’s gradual shift to liberalism. This rate of shift increased
over time. He supported the liberalisation of trade, was a liberal
internationalist and opposed 1870s Disraelite policy, as one would
expect of a liberal.

This is, however, an incomplete picture. Consider that he said “I am an
out and out inequalitarian”, would likely have opposed women’s
sufferage, caused the 1866 Reform Bill to fail by its excessive
moderation, bombarded Alexandria and advocated war with Bismarck in
1964.

### Religion

Every morning Gladstone went to Anglican communion at 8:30. He wrote on
the relationship between Church and state in 1836.

The question here is whether his politics can be reduced to his
religious beliefs. He had two desks - one for religion and another for
politics. **Optically this says one thing, but the value of this optical
impression is of course unclear.** If he were truly religious, why
disestablish the Irish church in 1869?

### Ireland

One can make the case that his policy on Ireland was indicative of his
liberalism. Recall his attempt in 1868 to disestablish the church. In
1886, he attempted Home Rule, as he did again in 1893.

There is, however, an alternative explanation for his actions. In 1868
the only issue which united his party was Irish disestablishment. Home
Rule will be discussed later.

### Legacy

Does Gladstone invent liberalism or cause its death? In 1906, there were
400 liberal MPs - perhaps he laid the foundation for this.
Alternatively, Gladstone laid the foundation for the eventual demise of
liberal politics by the late 1920s.

### Historiography

Time and space can cause variance in views of historical figures. In
1903, the first book about him appears. Written by the Chief Secretary
for Ireland, John Morley, it is a “laudatory book”[^1]. Criticism was
staved off till the end of the first world war. The family sent his
papers to the British Library.

This leads to a number of complications due to scholarly activity. The
fundamentals stay - Gladstone is a positive and convincing fellow to
those who follow. J R Hammond in 1938 in *Gladstone and the Irish
Nation* has a vision of Gladstone provides one example of this.

In 1954 Philip Magnsu published another biography of Gladstone with a
little criticism. He was deprived of much source material since the
Gladstone family knew that he was agnostic. They feared that he might
not have understood Gladstone’s diary as a result of his agnosticism.

By the 1960s, the family decided that this was absurd. They made the
diary public and sent it to the Lambeth Palace Library. There, M R D
Foot and, after a few volumes, H C G Mathews edited the diary and
published in over a period of 15 years. The diaries contain 3 million
words. 21,000 books are mentioned. Interestingly, there are **(as would
likely be expected)** remarks about other people.

The diary contained a number of squiggles every day. It was discovered
that this corresponded to his visits to brothels. In his diary he
records that he never slept with these women. It is clear, however, that
the squiggles represent a sort of self-flaggelation. This was a tortured
man.

Gladstone is much more ordinary than we want him to be. He was a
political manipulator. His sanctimony irritated previous generations and
lead to their dislike of him. The diary’s publication from 1968 reveals
that he is not as extraordinary in some ways as was thought.

In the 1970s, some “revisionist” historiography claims that Gladstone
was not really a liberal. This is primarily due to disagreement over
religion’s importance to Gladstone. some attempt to revise the view of
his views. We modern people are unable to comprehend fully the
importance of religion to those who lived before us.

### Gladstone’s motives

A B Cooke and John Vincent write in *The Governing Passion* that
politicians discover policies so as to permit them to continue
governing, instead of the inverse. Gladstone as someone to be put on a
pedestal is a false Gladstone.

Consider that in the 1880-1895 Gladstone ministry, he tells his close
family that in his mind he is moving towards support for Home Rule in
Ireland. Not a word leaks out, until 1885, when his son, Herbert, who is
supposed to be incompetent, spread this to the press. This lead to a
controversy. Home Rule later failed. This is the conventional view.

Cooke and Vincent say that Chamberlain was a radical liberal, who hadn’t
attended university, was a Unitarian progressive, with a certain
imperialist view, and was hated by Gladstone passionately. Ireland was
the closest colony. Gladstone attempted to stop Chamberlain by granting
Home Rule to what was essentially the closest colony - Ireland.
Gladstone also underestimated Chamberlain. He preferred a non-imperial
liberalism.

### Conclusion

Had World War I not occurred, would we still have a liberal party today?
The liberals could well have taken the place of the European social
democrats, had Gladstone not poisoned their relationship with socialists
and Labour.

Professor Apsel concludes that “if one tries to read one’s history in a
historiographical way, as I tried, it will be more difficult but a damn
sight more interesting”.

[^1]: These words are, as far as I can recall, Professor Apsel’s,
    although they may be someone else’s too.