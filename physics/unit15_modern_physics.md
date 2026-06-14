# Unit 15: Modern Physics

> Exam Weight: 12--15% | ~14--22 Class Periods

## Topics

### 15.1 Quantum Theory and Wave-Particle Duality
- Light and all matter display a dual character, behaving as waves in some situations and as discrete particles in others
- Each quantum of electromagnetic energy — a photon — carries energy:
  $$E = hf = \frac{hc}{\lambda}$$
  where $h = 6.63 \times 10^{-34} \text{ J·s}$ is Planck's constant
- De Broglie proposed that any object with momentum $p$ has an associated matter wavelength:
  $$\lambda = \frac{h}{p} = \frac{h}{mv}$$
- For everyday macroscopic objects, $\lambda$ is so tiny that wave behavior is completely undetectable in practice
- Subatomic particles like electrons have a small enough momentum that their wavelength is measurable — for instance, electrons produce diffraction patterns
- The single-particle double-slit experiment is the clearest demonstration of duality: each individual particle registers as a localized dot, yet after many events the cumulative dot pattern reproduces the wave interference fringe pattern

### 15.2 The Bohr Model of Atomic Structure
- Bohr proposed that electrons are confined to discrete circular orbits around the nucleus, each orbit corresponding to a quantized value of angular momentum
- For a hydrogen atom, the allowed energies are:
  $$E_n = -\frac{13.6}{n^2} \text{ eV}$$
  where $n = 1, 2, 3, \ldots$ is the principal quantum number
- The most tightly bound configuration ($n = 1$) is the ground state with $E_1 = -13.6 \text{ eV}$
- Any level with $n \geq 2$ is an excited state — the energy is less negative (closer to zero) than the ground state
- Taking $n$ to infinity drives $E_n$ to zero, which defines the ionization threshold; 13.6 eV must be supplied to ionize a ground-state hydrogen atom
- When an electron jumps between levels, it either absorbs or emits a single photon whose energy precisely matches the gap:
  $$E_{\text{photon}} = |E_{\text{higher}} - E_{\text{lower}}| = hf$$

### 15.3 Emission and Absorption Spectra
- **Emission spectrum**: when an excited atom releases energy, electrons fall to lower levels and emit photons of specific wavelengths; the resulting spectrum shows bright colored lines against a dark background
- **Absorption spectrum**: when white light passes through a cool gas, atoms absorb only the wavelengths matching their energy-level gaps, leaving dark lines on an otherwise continuous bright background
- Because each element has its own unique set of energy levels, its spectral lines act as a distinctive signature for identification
- Hydrogen's spectral lines group into series based on the final level of the transition:
  - **Lyman series**: electrons land on $n = 1$ (photons in the ultraviolet)
  - **Balmer series**: electrons land on $n = 2$ (photons in the visible range)
  - **Paschen series**: electrons land on $n = 3$ (photons in the infrared)
- The Rydberg formula gives the wavelength of any hydrogen line:
  $$\frac{1}{\lambda} = R_H \left(\frac{1}{n_f^2} - \frac{1}{n_i^2}\right)$$
  where $R_H = 1.097 \times 10^7 \text{ m}^{-1}$ is the Rydberg constant

### 15.4 Blackbody Radiation
- Every object warmer than absolute zero emits a continuous thermal radiation spectrum; the distribution of wavelengths depends only on the object's temperature
- **Wien's displacement law** locates the peak of this spectrum:
  $$\lambda_{\max} T = 2.898 \times 10^{-3} \text{ m·K}$$
  A hotter object peaks at a shorter wavelength, which is why a furnace glows blue-white rather than red as it is heated further
- **Stefan-Boltzmann law** gives the total power radiated per unit time:
  $$P = \sigma A T^4$$
  where $\sigma = 5.67 \times 10^{-8} \text{ W·m}^{-2}\text{·K}^{-4}$, $A$ is the surface area, and $T$ is the absolute temperature in kelvins
- Classical electrodynamics predicted that radiated power should grow without bound at short wavelengths — a failure known as the **ultraviolet catastrophe** because experimental spectra clearly do not diverge
- Planck's resolution was to postulate that electromagnetic energy can only be exchanged in discrete multiples $E = nhf$ ($n = 1, 2, 3, \ldots$), a hypothesis that fit the measured spectra perfectly

### 15.5 The Photoelectric Effect
- Illuminating a metal with sufficiently energetic light dislodges electrons from the surface; these freed electrons are called photoelectrons
- Einstein's energy balance for the process:
  $$E_{\text{photon}} = KE_{\max} + \phi$$
  equivalently: $KE_{\max} = hf - \phi$
- $\phi$ is the **work function** — a material-specific constant equal to the minimum energy required to pull one electron free from the metal surface
- **Threshold frequency**: $f_0 = \frac{\phi}{h}$; light below this frequency cannot dislodge electrons no matter how bright it is
- The **stopping voltage** $V_s$ is the smallest reverse potential that brings the fastest photoelectrons to rest:
  $$eV_s = KE_{\max} = hf - \phi$$
- Features that the classical wave model of light fails to account for:
  - The existence of a sharp threshold frequency
  - Emission begins the instant the light is turned on, with no measurable delay
  - $KE_{\max}$ rises with light frequency but is independent of light intensity
- How the photon model explains all of these:
  - A single photon delivers a packet of energy $hf$; if that packet is smaller than $\phi$, no electron escapes
  - Greater intensity means more photons arriving per second, which increases the electron current but does not change what any individual photon can do
  - A higher-frequency photon carries more energy per packet, directly raising $KE_{\max}$

### 15.6 Compton Scattering
- When an X-ray photon strikes a nearly free electron, it bounces off like a billiard ball: the photon loses energy and comes out at a longer wavelength, while the electron recoils
- The increase in photon wavelength depends on the scattering angle $\theta$:
  $$\Delta\lambda = \lambda' - \lambda = \frac{h}{m_e c}(1 - \cos\theta)$$
- The quantity $\frac{h}{m_e c} = 2.43 \times 10^{-12} \text{ m}$ is the electron's Compton wavelength, setting the scale of the wavelength shift
- The largest possible shift occurs at $\theta = 180°$ (the photon bounces straight back): $\Delta\lambda_{\max} = \frac{2h}{m_e c}$
- Photon momentum is:
  $$p = \frac{h}{\lambda} = \frac{E}{c}$$
- Compton's measurements confirmed that photons obey the same conservation laws of energy and momentum in collisions as classical particles do, providing strong evidence for the particle nature of light

### 15.7 Fission, Fusion, and Nuclear Decay
- **Mass-energy equivalence**: Einstein's $E = mc^2$ establishes that mass and energy are interconvertible; even a tiny mass converts to an immense amount of energy
- **Mass defect** $\Delta m$: when protons and neutrons come together to form a nucleus, the resulting nucleus is measurably lighter than the sum of its free constituent masses
- **Binding energy**: $E_b = \Delta m \cdot c^2$ quantifies how tightly the nucleus is held together — it equals the energy that would be needed to pull every nucleon completely apart
- A nucleus with a higher binding energy per nucleon is more stable; iron-56 occupies the peak of this curve
- **Nuclear fission**: striking a heavy nucleus such as uranium-235 with a neutron can cause it to split into two mid-sized nuclei
  - The split releases additional neutrons that can trigger further fissions, sustaining a **chain reaction**
  - Energy is released because the fragment nuclei sit higher on the binding-energy-per-nucleon curve than the original heavy nucleus
- **Nuclear fusion**: forcing two light nuclei (e.g., isotopes of hydrogen) together produces a heavier nucleus
  - This is the energy source of stars; extremely high temperatures are needed to give nuclei enough kinetic energy to overcome their mutual electrostatic repulsion and reach the range of the strong force
  - Energy is released because the product nucleus has more binding energy per nucleon than the two separate reactants
- Both processes liberate energy for the same underlying reason: the reaction products sit closer to the iron-56 peak on the binding-energy-per-nucleon curve than the starting materials do

### 15.8 Types of Radioactive Decay
- **Alpha decay** ($\alpha$): the nucleus ejects a helium-4 nucleus ($^4_2\text{He}$), also called an alpha particle
  $$^A_Z X \to ^{A-4}_{Z-2} Y + ^4_2\text{He}$$
  The daughter nucleus has a mass number 4 less and an atomic number 2 less than the parent
- **Beta-minus decay** ($\beta^-$): a neutron inside the nucleus transforms into a proton, ejecting an electron and an electron antineutrino
  $$^A_Z X \to ^{A}_{Z+1} Y + e^- + \bar{\nu}_e$$
  The mass number is unchanged; the atomic number increases by 1
- **Beta-plus decay** ($\beta^+$): a proton inside the nucleus transforms into a neutron, ejecting a positron and an electron neutrino
  $$^A_Z X \to ^{A}_{Z-1} Y + e^+ + \nu_e$$
  The mass number is unchanged; the atomic number decreases by 1
- **Gamma decay** ($\gamma$): a nucleus in an excited state sheds excess energy by emitting a high-energy photon while remaining the same element
  $$^A_Z X^* \to ^A_Z X + \gamma$$
- **Conservation in nuclear reactions**: both the mass number $A$ (total nucleon count) and the atomic number $Z$ (proton count) are separately conserved in every nuclear process
- **Half-life** $t_{1/2}$: the characteristic time needed for half the nuclei in any-sized sample to decay
  $$N = N_0 \left(\frac{1}{2}\right)^{t/t_{1/2}}$$
  equivalently: $N = N_0 \, e^{-\lambda t}$ where the decay constant $\lambda = \frac{\ln 2}{t_{1/2}}$
- Half-life describes the average behavior of a large ensemble; the moment at which any particular nucleus decays is fundamentally random and cannot be predicted

## Skills to Master

- Articulate wave-particle duality and cite specific experiments that reveal the wave-like and particle-like behavior of both light and matter
- Compute photon energy, frequency, wavelength, and momentum using Planck's relation and the photon momentum formula
- Find the de Broglie wavelength of a particle from its mass and velocity or its momentum
- Apply the Bohr hydrogen model to determine allowed energy levels and the energies of photons emitted or absorbed during transitions
- Differentiate emission and absorption spectra and connect each spectral line to a specific transition between energy levels
- Use Wien's displacement law and the Stefan-Boltzmann law to solve quantitative problems about blackbody radiation
- Analyze the photoelectric effect with the photon model to find threshold frequency, maximum kinetic energy of ejected electrons, and stopping voltage
- Explain the mechanism of Compton scattering and compute the wavelength shift for a given scattering angle
- Use $E = mc^2$ to calculate energy released or absorbed in nuclear reactions involving a mass defect
- Compare fission and fusion in terms of which nuclei are involved and how binding energy per nucleon governs the energy released
- Write balanced nuclear decay equations and identify the conservation rules that apply to each type (alpha, beta, gamma)
- Apply the half-life relationship to determine what fraction of a radioactive sample survives after a specified time

## Core Concepts

1. Light (and all electromagnetic radiation) exhibits a dual nature: it propagates as a wave but interacts with matter as discrete photons that carry energy $E = hf$ and momentum $p = h/\lambda$ yet have zero rest mass
2. Matter particles, too, have an associated wavelength given by $\lambda = h/p$; this wave character is detectable only when the particle's momentum is very small, as it is for electrons
3. Bohr's model restricts hydrogen's electron to specific orbits, giving quantized energy levels $E_n = -13.6/n^2$ eV; every spectral line arises from a jump between two of these levels
4. The spectrum of thermal radiation from a heated object depends solely on temperature; Planck's insight that energy is emitted in discrete quanta $E = nhf$ resolved the classical prediction of infinite emission at short wavelengths
5. The photoelectric effect reveals that light delivers energy in indivisible photon packets — no matter how intense the light, no electron escapes unless each photon's energy $hf$ exceeds the work function; it is frequency, not intensity, that sets the maximum kinetic energy of ejected electrons
6. In Compton scattering, an X-ray photon exchanges momentum with a free electron in exactly the same way two billiard balls would collide, confirming that photons carry real momentum
7. When nucleons assemble into a nucleus, the resulting "missing" mass (mass defect) converts into binding energy via $E = mc^2$; whether a reaction releases energy depends on whether the products sit higher on the binding-energy-per-nucleon curve than the reactants
8. Radioactive nuclei decay at rates governed purely by nuclear physics: the population of undecayed nuclei falls exponentially in time with a fixed half-life, and every decay event conserves both mass number and atomic number

## Key Equations

### Photon Energy and Momentum

$$E = hf = \frac{hc}{\lambda}$$

$$p = \frac{h}{\lambda} = \frac{E}{c}$$

### de Broglie Wavelength

$$\lambda = \frac{h}{p} = \frac{h}{mv}$$

### Bohr Model (Hydrogen)

$$E_n = -\frac{13.6}{n^2} \text{ eV} \quad (n = 1, 2, 3, \ldots)$$

$$E_{\text{photon}} = |E_f - E_i| = hf$$

### Rydberg Formula

$$\frac{1}{\lambda} = R_H \left(\frac{1}{n_f^2} - \frac{1}{n_i^2}\right) \quad (R_H = 1.097 \times 10^7 \text{ m}^{-1})$$

### Blackbody Radiation

$$\lambda_{\max} T = 2.898 \times 10^{-3} \text{ m·K} \quad \text{(Wien's displacement law)}$$

$$P = \sigma A T^4 \quad (\sigma = 5.67 \times 10^{-8} \text{ W·m}^{-2}\text{·K}^{-4}) \quad \text{(Stefan-Boltzmann law)}$$

### Photoelectric Effect

$$KE_{\max} = hf - \phi$$

$$f_0 = \frac{\phi}{h} \quad \text{(threshold frequency)}$$

$$eV_s = KE_{\max} \quad \text{(stopping voltage)}$$

### Compton Scattering

$$\Delta\lambda = \frac{h}{m_e c}(1 - \cos\theta) \quad \left(\frac{h}{m_e c} = 2.43 \times 10^{-12} \text{ m}\right)$$

### Mass-Energy Equivalence

$$E = mc^2$$

$$E_b = \Delta m \cdot c^2 \quad \text{(binding energy)}$$

### Radioactive Decay

$$N = N_0 \left(\frac{1}{2}\right)^{t/t_{1/2}}$$

$$\lambda_{\text{decay}} = \frac{\ln 2}{t_{1/2}}, \quad N = N_0 \, e^{-\lambda_{\text{decay}} t}$$

## Key Terminology

| Term | Definition |
|------|-----------|
| **Photon** | The elementary particle of light and all electromagnetic radiation; it carries energy $E = hf$ and momentum $p = h/\lambda$ but has no rest mass |
| **Planck's constant** | The universal proportionality constant $h = 6.63 \times 10^{-34} \text{ J·s}$ that links a photon's energy to its frequency |
| **de Broglie wavelength** | A wavelength $\lambda = h/p$ that quantum mechanics associates with any moving particle as a consequence of its momentum |
| **Wave-particle duality** | The observation that light and matter each display wave behavior in some experiments (e.g., diffraction) and particle behavior in others (e.g., localized detection) |
| **Ground state** | The configuration of lowest possible energy for an atom; for hydrogen this is the $n = 1$ level |
| **Excited state** | Any atomic configuration with more energy than the ground state; for hydrogen, any level with $n \geq 2$ |
| **Work function** | The threshold energy $\phi$ that must be supplied to free one electron from the surface of a particular metal |
| **Threshold frequency** | The critical light frequency $f_0 = \phi/h$ below which no electrons are ejected regardless of how bright the light is |
| **Stopping voltage** | The reverse voltage $V_s$ applied in a photoelectric experiment just sufficient to halt even the fastest ejected electrons; $eV_s = KE_{\max}$ |
| **Blackbody** | A theoretical perfect absorber and emitter of radiation; its emission spectrum depends only on temperature and peaks at a wavelength given by Wien's law |
| **Mass defect** | The amount by which the mass of a completed nucleus is less than the combined mass of its constituent protons and neutrons taken separately |
| **Binding energy** | The energy released when a nucleus forms from free nucleons, equal to the mass defect multiplied by $c^2$; equivalently, the energy needed to completely dismantle the nucleus |
| **Half-life** | The time interval $t_{1/2}$ after which exactly half of any initial number of radioactive nuclei have decayed, on average |
| **Fission** | A nuclear process in which a massive nucleus (e.g., uranium-235) breaks apart into two smaller nuclei, releasing energy because the fragments are more tightly bound per nucleon |
| **Fusion** | A nuclear process in which two lightweight nuclei merge into a heavier one, releasing energy because the product is more tightly bound per nucleon than the original pair |

## Common Misconceptions

1. **Photons must have mass if they carry momentum** -- Incorrect. Photon momentum is $p = E/c = h/\lambda$, derived from relativistic energy relations rather than from mass. Photons have strictly zero rest mass; the classical formula $p = mv$ simply does not apply to them.
2. **Brighter light ejects faster photoelectrons** -- Incorrect. Raising the intensity sends more photons per second at the metal, which boosts the number of ejected electrons (photocurrent) but leaves the maximum kinetic energy of each electron unchanged. Only a higher photon frequency raises $KE_{\max}$.
3. **Electrons follow well-defined circular orbits around the nucleus** -- The Bohr model assumes circular orbits as a useful mathematical approximation. Modern quantum mechanics instead describes each electron's position as a probability cloud. The Bohr model successfully predicts hydrogen energy levels but gives a misleading picture of where the electron actually is.
4. **Heating a radioactive sample or placing it under high pressure will accelerate its decay** -- Incorrect. Nuclear decay rates are set by the strong nuclear force deep inside the nucleus and are completely insensitive to external conditions such as temperature, pressure, or chemical environment.
5. **After two half-lives, a radioactive sample is completely gone** -- Incorrect. Each half-life removes half of whatever amount remains. After two half-lives, one-quarter of the original sample is still present. The amount declines exponentially and theoretically never reaches exactly zero; after $n$ half-lives the remaining fraction is $(1/2)^n$.
6. **Any nucleus can serve as fuel for either fission or fusion** -- Incorrect. The binding-energy-per-nucleon curve peaks at iron-56. Fission releases energy only for nuclei heavier than iron (splitting them moves toward the peak); fusion releases energy only for nuclei lighter than iron (merging them also moves toward the peak). Applying the wrong process to iron or near-iron nuclei would absorb energy rather than release it.
7. **The electron emitted in beta-minus decay was sitting inside the nucleus beforehand** -- Incorrect. Stable electrons cannot exist inside a nucleus. In beta-minus decay, a neutron is converted into a proton, and the electron (along with an antineutrino) is newly created in that instant by the weak nuclear force.

## Units and Dimensional Analysis

| Quantity | SI Unit | Dimension |
|----------|---------|-----------|
| Energy | J (joule); also eV ($1 \text{ eV} = 1.602 \times 10^{-19} \text{ J}$) | [M][L]$^2$[T]$^{-2}$ |
| Frequency | Hz (hertz) = s$^{-1}$ | [T]$^{-1}$ |
| Wavelength | m (meter) | [L] |
| Planck's constant $h$ | J·s | [M][L]$^2$[T]$^{-1}$ |
| Momentum | kg·m/s | [M][L][T]$^{-1}$ |
| Work function $\phi$ | J or eV | [M][L]$^2$[T]$^{-2}$ |
| Electric potential (stopping voltage) | V (volt) = J/C | [M][L]$^2$[T]$^{-3}$[I]$^{-1}$ |
| Mass | kg; also u ($1 \text{ u} = 1.661 \times 10^{-27} \text{ kg} = 931.5 \text{ MeV}/c^2$) | [M] |
| Half-life | s (second) | [T] |
| Decay constant $\lambda$ | s$^{-1}$ | [T]$^{-1}$ |
| Stefan-Boltzmann constant $\sigma$ | W·m$^{-2}$·K$^{-4}$ | [M][T]$^{-3}$[Θ]$^{-4}$ |
| Temperature | K (kelvin) | [Θ] |
