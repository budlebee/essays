
> "We know the past but cannot control it. We control the future but cannot know it." - Claude Shannon

# Connection

 *Connections change the world.* Due to the limitations of human cognitive ability, the size of the naturally occurring group does not exceed 150, called Dunbar’s number[1]. But humans in modern society live in a larger group than that. The reason why human groups can exceed the Dunbar’s number is that humans are connected to each other by sharing information[2]. Religion is a good example. Religion connects people through the same belief. The development of civilization and religion in history are inseparable. Mankind was able to achieve a civilization distinct from other primates by developing common beliefs. Believe or not, *'Let there be light'* changed the world. 
 
Humans have developed various information sharing methods. *Gutenberg’s printing press, Marconi’s wireless telegraphy, emergence of the world wide web*... Science and technology have gradually increased the size of connections and expanded the horizon of the world. Now mankind is going to connect the world using quantum entanglement. Entanglement is a unique phenomenon that only appears in quantum systems. It is possible to create new information sharing methods that have never existed before.

# Entanglement

When two or more systems link up in a certain way and cannot be described independently of the state of the others, we call it \textit{Entanglement}. Entanglement is represented by kronecker product and superposition of vectors. 

Most famous entangled state is the Bell state, as follows:

$$
\ket{\Psi^+_{AB}} = \frac{1}{\sqrt{2}}(\ket{0_A1_B}+\ket{1_A0_B}) 
$$

0 and 1 is two dimensional orthonomal basis. The meaning of this equation is that if Alice(A) measures 0, Bob(B) will measure 1, and if Alice measures 1, Bob will measure 0. Quantum information can be transmitted using the Bell state. It is called \textit{Quantum Teleportation}[3]. Let's say the quantum state that Alice wants to send to Bob as follows $\ket{\psi_C}=\alpha\ket{0_C}+\beta\ket{1_C}$.

Then whole system is:

$$
\ket{\psi_C}\otimes\ket{\Psi^+_{AB}}\newline
 =(\alpha\ket{0_C}+\beta\ket{1_C}) \otimes(\frac{1}{\sqrt{2}}(\ket{0_A1_B}+\ket{1_A0_B})) \newline
=\frac{1}{\sqrt{2}}(\alpha\ket{0_C0_A1_B}+\alpha\ket{0_C1_A0_B}+\beta\ket{1_C0_A1_B}+\beta\ket{1_C1_A0_B})

$$
Alice does projection measurement to $\ket{\Psi^+_{CA}}=\frac{1}{\sqrt{2}}(\ket{0_C1_A}+\ket{1_C0_A})$. By orthogonality, the state becomes:

$$
\alpha\ket{0_B}+\beta\ket{1_B}
$$

By measuring local state CA, Alice can send quantum state information to Bob.

So how can we implement the Bell state physically? We use Spontaneous Parametric Down-Conversion(SPDC), non-linear optical process.

# Light

SPDC is a photon spontanously splits into two other photons of lower frequencies[3]. If you lase a pump beam at a crystal that causes an SPDC phenomenon, you will get two lights that meet the following conditions:
$$
w_p = w_s+w_i\newline
\vec{k_p}=\vec{k_s}+\vec{k_i}
$$
where the subscript p refers to the *pump* beam, s and i refer to the *signal* and *idler* beams. The process is said to be degenerate if the down converted photons have the same free space wavelength. In general, the photons of a down-converted pair exit the crystal non-collinearly, in different directions which satisfy the momentum conservation.

![fig1](./fig1.png)
a) Feynman diagram of Spontaneous Parametric Down-Conversion(SPDC). b) Energy conservation of SPDC. c) Momentum conservation of SPDC. d) Experimental setup of SPDC using beta-Barium Borate(BBO). 

By adjusting the angle between BBO crystal and pump beam, the signal beam and idler beam can overlap (figure 1) [4]. The polarization of the signal and idler are perpendicular to each other in type-2 SPDC. Ideally, It is impossible to distinguish which light comes from which. So the $\frac{1}{\sqrt{2}}(\ket{HV}+\ket{VH})$ state is created. If we encode H polarization as 0 and V polarization as 1, the equation (1) is implemented.

There are many ways to create a Bell state and deliver quantum information. *'Let there be light'* will play a important role in new information era.

 # reference

 1. Dunbar, R. I. M. (1992). "Neocortex size as a constraint on group size in primates". Journal of Human Evolution. 22 (6): 469–493. doi:10.1016/0047-2484(92)90081-J
 2. Palmer, C. Harari, Yuval Noah. 2015. Sapiens: A Brief
History of Humankind.. Evolutionary Studies In Imagina-
tive Culture. 1, 237-244 (2017),
3. Bennett, C., Brassard, G., Cr epeau, C., Jozsa, R., Peres,
A. & Wootters, W. Teleporting an unknown quantum
state via dual classical and Einstein-Podolsky-Rosen chan-
nels. Phys. Rev. Lett.. 70, 1895-1899 (1993,3),
4. Christophe Couteau (2018) Spontaneous parametric down-conversion, Contemporary Physics, 59:3, 291-304, DOI: 10.1080/00107514.2018.1488463