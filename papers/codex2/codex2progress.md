# Codex2 Progress

Running reverse-chronological research notes for the Codex2 lane.

Purpose:
- preserve what was actually learned, not just what was run
- make promotion decisions for the main paper easier later
- record both positive signals and clean non-promotions

## 2026-03-15 - RFTP-1.58 E6-to-SU(3) Sector Extraction Probe

### Ticket
`RFTP-1.58 - E6-to-SU(3) Sector Extraction Probe`

### Objective
Test whether the bounded E6-style chart family contains a stable gauge-hosting subprojection that isolates the gauge sector more tightly than the full bridge chart.

### Result
Classification: `gauge_sector_extraction_partial`

Bottom line:
A real gauge-sector subprojection exists, but it is still best described as a bounded partial extraction rather than a closed SU(3)-like sector chart.
The strongest gauge-only chart was not the canonical `curvature_weighted_host_pair` axis.
It was the rival-family spine axis:
`host_depth`.

### Main Findings

#### 1. The best gauge-only sector chart is one-dimensional
Best gauge-only chart:
- `host_depth_axis`

Source chart family:
- `spine_interface_pair`

Best sector axes:
- `host_depth`

Interpretation:
The gauge-hosting subset does compress into a simpler one-axis chart.
That is a real sector-extraction signal.
But it comes from the bounded chart family as a whole, not from a uniquely privileged canonical axis.

#### 2. The extracted gauge chart is tighter than the full bridge references
Gauge-only quality:
- `0.7642`

Gauge-only compression:
- `0.8920`

Gauge-only minimum separation:
- `0.3561`

Gauge-only vs full bridge quality gap:
- `+0.2034`

Interpretation:
For the gauge-hosting subset, the one-axis `host_depth` extraction is cleaner than carrying the full bridge chart.
That supports a bounded sector chart rather than only a bridge-wide chart.

#### 3. The spine-local gauge axis is real but not fully strong enough for promotion
Best local spine axis score:
- `0.8086`

Host pair compactness:
- `1.0000`

Shell order margin:
- `0.3331`

Interpretation:
The hosting spine does show a meaningful local gauge axis.
But the aggregate local-axis score still falls short of the stronger threshold that would justify a promoted SU(3)-like subprojection claim.

#### 4. The canonical bridge axis is not the best gauge extractor
`curvature_host_axis` quality:
- `0.6829`

`curvature_host_axis` minimum separation:
- `0.1091`

Interpretation:
The best bridge chart and the best gauge-sector chart are not the same object.
That is an important structural clue:
the gauge sector appears to prefer a more spine-local depth coordinate than the full bridge prefers.

### Promotion Boundary
Promoted from this ticket:
- none

Partial only:
- existence of a bounded gauge-sector subprojection inside the E6-style chart family
- spine-local one-axis gauge organization on `host_depth`

Not promoted:
- literal SU(3) recovery
- a closed sector chart
- any claim that the gauge sector is uniquely extracted from the canonical bridge chart alone

### Best next use
Use this result to:
- write the gauge-sector extraction as a bounded local chart note
- keep the chart-family caveat explicit
- test whether the `host_depth` sector axis transports and stabilizes under a dedicated SU(3)-side transport pass

## 2026-03-15 - RFTP-1.56 E6 Chart Uniqueness and Alternative Coordinate Rival Test

### Ticket
`RFTP-1.56 - E6 Chart Uniqueness and Alternative Coordinate Rival Test`

### Objective
Test whether the locked reduced bridge chart is genuinely unique, or whether a nearby rival chart family performs nearly as well.

### Result
Classification: `best_chart_real_but_not_unique`

Bottom line:
`curvature_weighted_host_pair` remains the best reduced bridge chart, but the lead over the nearest rival is modest rather than decisive.
The strongest alternative is still the simpler `spine_interface_pair`, so uniqueness language should remain bounded.

### Main Findings

#### 1. The best chart stayed best across the important bridge slices
Winner:
- `curvature_weighted_host_pair`

Runner-up:
- `spine_interface_pair`

Slice wins for the winner:
- `3`

Interpretation:
The winning chart is not an accident of a single metric.
It stayed on top across the bridge-relevant slice comparisons and retained the best overall dual-host balance.

#### 2. The winner's edge is real, but narrow
Quality margin over runner-up:
- `0.0085`

Non-stress slice-score margin:
- `0.0097`

Control-gap margin:
- `0.0135`

Balance margin:
- `0.0239`

Interpretation:
The chart does separate from the nearest rival, but not by enough to claim a uniquely recovered coordinate basis.
The safe language is "best current bounded chart," not "the only real chart."

#### 3. The rival family still matters
Winner quality score:
- `0.7504`

Runner-up quality score:
- `0.7419`

Winner non-stress slice score mean:
- `0.8166`

Runner-up non-stress slice score mean:
- `0.8068`

Interpretation:
The bridge seems to support a small family of reasonable reduced charts.
The curvature-weighted chart is best because it balances gauge and weak structure slightly better, not because all competitors collapse.

### Promotion Boundary
Promoted from this ticket:
- `curvature_weighted_host_pair` as the current best reduced bridge chart

Partial only:
- uniqueness of the winning chart
- any claim that the reduced chart is a uniquely recovered intermediate basis

Not promoted:
- chart-family collapse to a single inevitable coordinate system

### Best next use
Use this result to:
- keep `curvature_weighted_host_pair` as the canonical reduced chart
- keep an explicit rival-chart caveat in the E6 writeup
- treat the current result as a best-chart lock, not a uniqueness theorem

## 2026-03-15 - RFTP-1.55 E6 Projection Coordinate Writeup

### Ticket
`RFTP-1.55 - E6 Projection Coordinate Writeup`

### Objective
Lock the reduced bridge chart into manuscript-safe form with explicit promotion boundaries and non-promotion language.

### Result
Classification: `bounded_e6_coordinate_chart_locked`

Bottom line:
The hosting bridge now has a locked reduced chart:
`curvature_weighted_host_pair` with axes `curvature_host | interface_progress`.
It is strong enough to reuse as a bounded intermediate coordinate system, but not to promote as a literal E6 recovery.

### Main Findings

#### 1. The reduced chart is now promoted in bounded language
Locked chart:
- `curvature_weighted_host_pair`

Axes:
- `curvature_host | interface_progress`

On-manifold score:
- `0.9522`

Observable simplification:
- `0.8760`

Transport stability:
- `0.9095`

Interpretation:
This is no longer just a good local fit.
It is strong enough to treat as the canonical bounded host-manifold chart for the current bridge.

#### 2. Observable lock and transport both stayed above the writeup threshold
Anchor-like gauge lock:
- `0.8979`

Anchor-like weak lock:
- `0.7735`

Conservative joint bridge score:
- `0.8769`

Minimum non-stress control gap:
- `0.0252`

Interpretation:
The chart preserves the useful part of the bridge under bounded transport and remains better than the clearly non-bridge alternatives on the slices where the bridge is supposed to live.

#### 3. Off-manifold behavior still acts like a real boundary lock
Off-manifold joint bridge score:
- `0.6764`

Off-manifold weak lock:
- `0.0000`

Interpretation:
The chart still fails the right way when pushed wedgeward.
That keeps the reduced-coordinate interpretation honest and bounded.

### Promotion Boundary
Promoted from this ticket:
- bounded reduced chart language for `curvature_weighted_host_pair`
- bounded observable lock on the reduced chart
- bounded transport support
- off-manifold contrast behavior

Not promoted:
- literal E6 algebra recovery
- complete group-theoretic derivation
- uniqueness of the chart
- wedgeward completion of the reduced chart

### Best next use
Use this result to:
- write the E6 bridge in chart language instead of only route language
- keep the interpretation explicitly geometric and bounded
- test rival-chart uniqueness before any stronger intermediate-layer claim

## 2026-03-15 - RFTP-1.54 E6 Coordinate Transport and Observable Lock

### Ticket
`RFTP-1.54 - E6 Coordinate Transport and Observable Lock`

### Objective
Test whether the reduced coordinates identified for the bounded E6-like hosting bridge transport across bounded slice variants and preserve the current gauge/weak observable lock.

### Result
Classification: `observable_lock_transport_supported`

Bottom line:
The best reduced chart does transport as a bounded observable-lock object.
It preserves the gauge/weak hosting organization across anchor-like, non-anchor, and conservative perturbation slices, and it fails only when deliberately pushed off-manifold toward the wedge-side detour.

### Main Findings

#### 1. The best reduced chart keeps the host manifold coherent in bounded slices
Best transported chart:
- `curvature_weighted_host_pair`

Anchor-like manifold score:
- `0.9522`

Conservative perturbation joint bridge score:
- `0.8769`

Interpretation:
The best chart is not just a one-slice fit.
It continues to organize the locked host objects under the conservative bridge extensions that already survived the 1.52 stress test.

#### 2. Gauge and weak locks survive the non-stress slices
Anchor-like gauge lock:
- `0.8979`

Anchor-like weak lock:
- `0.7735`

Non-anchor weak lock:
- `0.7735`

Interpretation:
The transport story is strongest on the observable side.
Even when the slice is weak-only on the candidate side, the reduced chart still keeps the weak-host structure locked on-manifold.

#### 3. Off-manifold stress behaves like a true contrast, not a hidden failure
Off-manifold joint bridge score:
- `0.6764`

Off-manifold weak lock:
- `0.0000`

Off-manifold control gaps:
- vs `mixed_bridge_pair`: `-0.1784`
- vs `bridge_adjacency_depth`: `-0.0969`

Interpretation:
The chart degrades exactly where it should:
when the route is forced wedgeward into mixed geometry.
That supports the bounded-manifold interpretation rather than weakening it.

#### 4. The chart still beats the non-E6-like control coordinates in the non-stress slices
Minimum non-stress control gap:
- `0.0252`

Anchor-like control gaps:
- vs `mixed_bridge_pair`: `0.1895`
- vs `bridge_adjacency_depth`: `0.2757`

Interpretation:
The best chart is not only coherent internally.
It remains better than the clearly non-bridge coordinate choices on the slices where the bridge is supposed to live.

### Promotion Boundary
Promoted from this ticket:
- bounded observable-lock transport for the best reduced chart
- off-manifold stress as an explicit contrast case

Partial only:
- stronger claim that the reduced chart is a globally reusable intermediate projection layer

Not promoted:
- a caveat-free transport law
- any claim that wedgeward detours belong to the reduced host chart

### Best next use
Use this result to support:
- bounded transport wording for the best reduced chart
- a writeup that treats the coordinate system as a reusable host-manifold chart, but not yet as a fully promoted intermediate layer

## 2026-03-15 - RFTP-1.53 E6 Projection Coordinate Identification

### Ticket
`RFTP-1.53 - E6 Projection Coordinate Identification`

### Objective
Identify the smallest stable reduced coordinate system that describes the bounded E6-like hosting bridge more cleanly than nearby off-manifold control charts.

### Result
Classification: `reduced_bridge_coordinates_partial`

Bottom line:
A real reduced chart was found, but it should still be described as a bounded local bridge chart rather than a fully locked projection layer.
The strongest basis was not the naive spine/interface pair; it was a curvature-weighted host coordinate paired with interface progression.

### Main Findings

#### 1. The best reduced chart is two-dimensional and bridge-specific
Best chart:
- `curvature_weighted_host_pair`

Axes:
- `curvature_host | interface_progress`

Quality score:
- `0.7504`

Interpretation:
The bridge does compress into a small chart.
But the best basis still leans on curvature-weighted hosting geometry rather than giving a fully clean minimal projection language.

#### 2. The on-manifold compression is strong
Best on-manifold score:
- `0.9522`

Effective dimension:
- `1.0014`

Observable simplification:
- `0.8760`

Interpretation:
The hosting bundle is close to one reduced direction in this chart, and the gauge/weak hosting picture becomes substantially cleaner there.

#### 3. Control separation is real but not overwhelming
Best-control gap:
- `0.0703`

Best control bundle:
- `core_shell_controls`

Runner-up chart:
- `spine_interface_pair`, quality `0.7419`

Interpretation:
The reduced chart is genuinely better than nearby control bases, but not by a huge enough margin to claim that the reduced coordinates are fully unique or fully locked.

#### 4. The mixed and bridge-adjacency controls behave the way they should
`mixed_bridge_pair`:
- quality `0.5807`
- control gap `-0.1017`

`bridge_adjacency_depth`:
- quality `0.5482`
- control gap `-0.1544`

Interpretation:
The off-manifold and bridge-only control coordinates fail in the expected way.
That helps confirm the best chart is not just an arbitrary low-dimensional fit.

### Promotion Boundary
Promoted from this ticket:
- a small reduced chart exists for the bounded hosting bridge

Partial only:
- the current best basis as the preferred E6-style coordinate chart

Not promoted:
- a uniquely identified minimal projection basis
- a literal E6 coordinate recovery

### Best next use
Use this result as the coordinate candidate to transport and stress-test, not yet as final projection language.

## 2026-03-15 - RFTP-1.52 E6 Bridge Stress Test Under Host Perturbation

### Ticket
`RFTP-1.52 - E6 Bridge Stress Test Under Host Perturbation`

### Objective
Test whether the bounded E6-like hosting bridge survives controlled perturbations of host boundaries, route definitions, candidate slices, and adjacency thresholds.

### Result
Classification: `e6_bridge_robust_with_caveats`

Bottom line:
The bridge survives conservative host perturbations.
It weakens only when the route is pushed into wedgeward mixed geometry or when the host set is expanded into higher-risk shell structure.
So the bridge is usable, but it should stay described as a bounded host-defined object.

### Main Findings

#### 1. Conservative host perturbations preserve the bridge
Conservative boundary coherence ratio:
- `0.8583`

Canonical route survival threshold:
- up to `0.65`

Conservative minimum joint advantage:
- `0.2275`

Conservative minimum weak advantage:
- `0.3296`

Interpretation:
The locked bridge is not just one brittle exact boundary choice.
It stays intact under contraction to the host objects, expansion into the outer shell, and extension toward the bend ridge.

#### 2. The expected failures are off-manifold
Weakest full-bridge route case:
- `all_aligned::wedgeward_detour`

Metrics:
- joint advantage: `0.1261`
- weak advantage: `-0.1767`

Most stressful boundary expansion:
- `expand_spine_fragility_shell`

Metrics:
- coherence ratio vs baseline: `0.7733`

Interpretation:
The bridge does not fail randomly.
It weakens exactly when we steer the route into mixed wedge-side geometry or dilute the host set with higher-risk fragility-shell structure.

#### 3. Candidate slices do not break the bridge by themselves
Verified-only canonical route:
- joint advantage: `0.3678`

Scale-caveated-only canonical route:
- weak advantage: `0.3833`

Non-anchor additions canonical route:
- weak advantage: `0.3296`

Interpretation:
The bridge is not being held together by one narrow candidate slice.
The candidate-side stress only turns negative when the route itself leaves the promoted host manifold.

### Promotion Boundary
Promoted from this ticket:
- the bridge is robust under conservative host perturbations

Partial only:
- stronger invariance to aggressive host-boundary changes
- stronger invariance to wedgeward route detours

Not promoted:
- a host-definition-insensitive bridge law
- a caveat-free manifold claim

### Best next use
Use this result to justify:
- bounded bridge language in the E6 note
- projection-coordinate probing on the conserved host manifold


## 2026-03-15 - RFTP-1.51 E6 Bridge Writeup and Promotion Boundary Lock

### Ticket
`RFTP-1.51 - E6 Bridge Writeup and Promotion Boundary Lock`

### Objective
Convert the E6 bridge probe and relation results into a manuscript-safe synthesis that promotes the stable bridge objects while explicitly locking the non-promoted claims.

### Result
Classification: `bounded_e6_bridge_locked`

Bottom line:
The bridge can now be written up cleanly in bounded geometric language.
The hosting spine and interface strip are promoted bridge objects, the manifold and gauge-to-weak bridge remain partial, and literal E6 recovery is still explicitly non-promoted.

### Main Findings

#### 1. The bridge objects are now locked cleanly
Central hosting spine:
- coherence: `0.9275`
- transport alignment: `0.9085`

Core-to-core interface strip:
- coherence: `0.9633`
- transport alignment: `0.9583`

Hosting manifold aggregate:
- coherence: `0.8274`
- shared transport alignment: `0.9334`

Interpretation:
The bridge is not one vague metaphor anymore.
It now has specific locked objects with explicit promotion boundaries.

#### 2. The strongest bridge statement is manuscript-safe
Canonical wording:
- The central hosting spine and core-to-core interface strip form a coherent reduced hosting manifold within the broader E8-derived atlas. Gauge and weak observables tighten substantially on this manifold relative to off-host controls, supporting an E6-like intermediate bridge interpretation in bounded geometric language.

Supporting metrics:
- coherence advantage: `0.2032`
- gauge on-host advantage: `0.5056`
- weak on-host advantage: `0.3833`
- joint on-host advantage: `0.2963`

#### 3. Candidate caveats are now explicit, not hidden
Aligned candidates:
- `10`

Scale-caveated aligned candidates:
- `6`

Quarantined holdouts:
- `color_sector_su3_boundary_echo_exp04`
- `casimir_dim_weighted_5_over_23_exp06`
- `casimir_alpha2_h_match_exp06`

Provenance-limited but not aligned:
- `su3_boundary_invariant_02191_synthesis`
- `weinberg_threshold_mu_star_synthesis`

Interpretation:
The bridge result is strong, but it is still candidate-set bounded.
That limitation is now part of the locked note rather than something implicit.

#### 4. Wedge exclusion is now part of the bridge lock
Wedge status:
- mixed transition-associated terminus

Wedge transport signal:
- `0.0000`

Interpretation:
The bridge does not pass through the wedge as a host region.
That closes the door on wedge-as-host language for this note.

### Promotion Boundary
Promoted from this ticket:
- central hosting spine as a stable gauge-host bridge object
- core-to-core interface strip as a stable weak-host bridge object
- on-host gauge relation lock
- on-host weak relation lock
- wedge exclusion from the bridge

Partial only:
- hosting manifold as a reduced bridge object
- gauge-to-weak bridge
- bounded E6-like interpretation

Not promoted:
- literal recovered E6 symmetry
- full E6-space relabeling
- wedge as a host region

### Best next use
Use this result to:
- cite a bounded E6-like bridge in the manuscript
- justify a stress test before any projection-coordinate search

## 2026-03-15 - RFTP-1.50 E6 Relation Lock on Gauge Weights and Weak Hosting

### Ticket
`RFTP-1.50 - E6 Relation Lock on Gauge Weights and Weak Hosting`

### Objective
Test whether the hosted observables on the spine/interface system exhibit constrained relational structure consistent with a bounded intermediate reduction layer.

### Result
Classification: `gauge_relations_supported_weak_bridge_partial`

Bottom line:
The on-host relation structure is real and stronger than nearby off-host controls.
But the bridge should still be described as a bounded intermediate-reduction clue, not as a closed E6 law.

### Main Findings

#### 1. Gauge relations are tight on the hosting spine
On-host gauge relation score:
- `0.9420`

Best off-host gauge control:
- `0.4364`

Gauge on-host advantage:
- `0.5056`

Interpretation:
The gauge-sector weights are not just cohosted.
On the hosting spine they lock into one shared host, one ordered simplex, and one transport-stable relation set.

#### 2. Weak-style relations are tight on the interface strip
On-host weak relation score:
- `0.9333`

Best off-host weak control:
- `0.5500`

Weak on-host advantage:
- `0.3833`

Weak ordering on the strip:
- `weak_sector_anchor_sin2_theta_w`
- `weak_sector_volume_weighted_cross_ratio_exp01`
- `e8_adjoint_cross_ratio_exp01`
- `weak_sector_resonance_peak_exp02`
- `weak_sector_resonance_band_mean_exp02`

Interpretation:
Weak-style observables are not just transition-hosted in general.
They form an ordered transition-affinity set on one common interface strip.

#### 3. The composite bridge relation is stronger on-host than off-host
Joint on-host bridge score:
- `0.8453`

Off-host route control:
- `0.5490`

Joint on-host advantage:
- `0.2963`

Interpretation:
Gauge and weak observables do not merely coexist on nearby geometry.
They form a tighter composite relation set on the locked hosting route than in nearby off-host controls.

### Promotion Boundary
Promoted from this ticket:
- on-host gauge relation structure is real
- on-host weak transition relation structure is real

Partial only:
- the gauge-to-weak bridge as an intermediate reduction clue

Not promoted:
- a literal E6 algebra claim
- a caveat-free unification law

### Best next use
Use this result to write:
- the hosted-observable relation layer of the E6 bridge note
- a bounded argument that hosting geometry is not accidental


## 2026-03-15 - RFTP-1.49 E6 Bridge Probe on Hosting Spine and Interface Strip

### Ticket
`RFTP-1.49 - E6 Bridge Probe on Hosting Spine + Interface Strip`

### Objective
Test whether `central_hosting_spine` and `core_to_core_interface_strip` behave like one coherent reduced hosting manifold rather than two unrelated Level-1 objects.

### Result
Classification: `hosting_manifold_partial_but_real`

Bottom line:
The hosting spine and interface strip are more coherent than generic Level-1 control bundles and do behave like a bounded reduced hosting manifold.
But the evidence is not yet sharp enough to promote a full E6-like intermediate layer.

### Main Findings

#### 1. The hosting bundle is unusually coherent
Hosting coherence score:
- `0.8274`

Best control score:
- `0.6241`

Coherence advantage:
- `0.2032`

Interpretation:
The hosting pair is not just an arbitrary adjacency.
It is more internally coherent than the best nearby non-host control bundle.

#### 2. The bridge edge is real and transport-stable
Gauge-to-interface bridge strength:
- `0.6606`

Shared transport alignment:
- `0.9334`

Gauge-to-interface support-risk step:
- `0.2789`

Interpretation:
The spine-to-strip connection behaves like a real bridge manifold, not a loose contact edge.

#### 3. The reduced-manifold claim stays bounded
Hosting bundle effective dimension:
- `1.0000`

Best control effective dimension:
- `1.0000`

Interpretation:
The hosting bundle does compress strongly, but so do some controls under the current coarse probe.
That is why the result stays partial rather than promoting all the way to an explicit E6-like manifold claim.

### Promotion Boundary
Promoted from this ticket:
- hosting objects are linked in a real bounded bridge structure

Partial only:
- reduced-manifold interpretation
- E6-like hosting language

Not promoted:
- a full intermediate-layer identification

### Best next use
Use this result as the geometric half of the E6 bridge argument:
- the manifold is real
- the strongest reason it stays partial is reduction sharpness, not lack of connectivity


## 2026-03-15 - RFTP-1.48 Level-1 Completeness Audit and Residual Gap Closure

### Ticket
`RFTP-1.48 - Level-1 Completeness Audit and Residual Gap Closure`

### Objective
Audit what remains unresolved in Level-1 and decide whether anything still blocks the E6 bridge.

### Result
Classification: `level1_complete_enough_for_e6_probe`

Bottom line:
There is no remaining Level-1 gap that looks material enough to block the E6 probe.
The map is not mathematically exhausted, but the unresolved pieces are now bounded local nuances rather than missing structural objects.

### Main Findings

#### 1. No blocking gap remains
Counts:
- residual gaps: `7`
- blocking gaps: `0`
- deferred gaps: `4`

Interpretation:
The current remaining issues are real, but they are not transition blockers.
They can be deferred unless the E6 bridge later fails.

#### 2. Formal completeness is now above the handoff threshold
Coverage scores:
- taxonomy: `0.98`
- internal core structure: `0.93`
- internal transition structure: `0.92`
- connectivity: `0.82`
- axis structure: `0.79`
- hosting organization: `0.97`
- overall Level-1: `0.9017`

Interpretation:
Level-1 is past the point where more pre-bridge cleanup is likely to change the main map.
The weakest area is still axis language, not topology or hosting organization.

#### 3. The remaining gaps are all bounded
Freeze permanently:
- `single_threshold_gate_story`
- `wedge_low_margin_internal_ambiguity`

Defer to later:
- `full_interface_normal_claim`
- `soft_core_lane_edges`

Revisit only if the E6 probe fails:
- `hosting_spine_full_symmetry_axis`
- `transition_lane_universality`

Safe to freeze:
- `aggregate_reference_resolution`

Interpretation:
The open items are now policy choices about how hard to push local structure, not missing atlas objects.

### Promotion Boundary
Promoted from this ticket:
- Level-1 is complete enough for the E6 bridge
- no unresolved object currently blocks the transition

Not promoted:
- a claim that Level-1 is fully closed with no deferred nuance
- a claim that interface-normal structure is already solved

### Best next use
Use this audit to justify:
- freezing the Level-1 atlas
- carrying the partial items only as deferred caveats
- moving cleanly into the E6 bridge lane


## 2026-03-15 - RFTP-1.47 Level-1 Atlas Synthesis and Promotion Boundary Lock

### Ticket
`RFTP-1.47 - Level-1 Atlas Synthesis and Promotion Boundary Lock`

### Objective
Fuse the whole Level-1 map into one locked atlas:
stable sector cores, transition surfaces, mixed zones, core submodes, transition lanes, adjacency graph, hosting routes, and axis structure.

### Result
Classification: `level1_atlas_locked`

Bottom line:
Level-1 can now be carried as one bounded atlas object.
The promoted geometry is no longer scattered across tickets.
It now lives in one manuscript-safe map with explicit promotion boundaries.

### Main Findings

#### 1. The atlas now contains all main Level-1 object families
Atlas object count:
- `19`

Promoted boundaries:
- `6`

Partial boundaries:
- `3`

Non-promoted boundaries:
- `1`

Interpretation:
The Level-1 map is now structured enough to bank as one object rather than a ticket sequence.

#### 2. The canonical Level-1 promotions are now locked
Promoted:
- stable sector cores
- transition surfaces
- mixed zones as non-core boundary objects
- core submodes
- weak interface-strip axis
- wedge as mixed boundary terminus

Partial:
- transition lanes as a family
- hosting routes
- hosting spine axis

Non-promoted:
- full interface-normal claim

Interpretation:
This is the final paper-safe boundary for Level-1 language before E6.

#### 3. The two route objects are now canonical atlas language
Gauge route:
- `central_hosting_spine -> core_to_core_interface_strip`
- strength `0.6606`

Weak route:
- `core_to_core_interface_strip -> bend_ridge -> mixed_wedge_terminus`
- strength `0.7764`

Interpretation:
The host geometry can now be explained in route language without implying a complete manifold transport law.

#### 4. The axis story is now cleanly bounded
Weak transition-side axis:
- promoted
- score `0.9000`

Hosting-spine axis:
- bounded ordered simplex lock only
- score `0.8333`

Interface-normal claim:
- non-promoted

Interpretation:
Transition-side hosting axis language is now stronger than the core-side symmetry claim.

### Promotion Boundary
Promoted from this ticket:
- Level-1 atlas as a unified object
- weak interface-strip axis
- wedge as mixed boundary terminus

Partial:
- route language
- hosting spine axis
- full lane family language

Not promoted:
- full interface-normal law

### Best next use
Use the atlas as:
- the canonical Level-1 geometry reference
- the fixed map for the E6 bridge
- the object future lanes should inherit rather than rebuild


## 2026-03-15 - RFTP-1.46 Symmetry-Axis Probe on Hosting Spine and Interface Strip

### Ticket
`RFTP-1.46 - Symmetry-Axis Probe on Hosting Spine and Interface Strip`

### Objective
Test whether the two strongest current hosting structures,
`central_hosting_spine` and `core_to_core_interface_strip`,
show evidence of deeper symmetry-axis organization.

### Result
Classification: `weak_axis_signal_supported`

Bottom line:
Both hosting objects show organized internal structure, but the cleaner current axis result is on the transition side.
The `core_to_core_interface_strip` behaves like a stable transition axis for weak-style observables.
The `central_hosting_spine` also shows axis-like organization, but the claim should stay narrower and core-host bounded.

### Main Findings

#### 1. The gauge-weight simplex stays locked on one shared hosting spine
Supported spine probes:
- `common_host_lock = 1.0000`
- `simplex_order_lock = 1.0000`
- `paired_shell_axis = 0.8013`
- `transport_persistence = 0.9085`
- `host_dispersion_lock = 0.0000`

Interpretation:
All promoted gauge weights still cohost on one shared spine in `nonwedge_domain`, and the current barycentric order remains intact there.

#### 2. The interface strip gives the strongest current axis result
Supported interface probes:
- `common_interface_lock = 1.0000`
- `bend_directionality = 0.8948`
- `transition_depth_order = 1.0000`
- `lane_transport_persistence = 0.9583`

Partial only:
- `interface_normal_chain = 0.0000`

Interpretation:
The interface strip does not yet promote as a full geometric normal-axis claim, but it does promote as an ordered transition axis object.

#### 3. Weak-style observables now have a stable ordered interface host
All current weak-style observables remain on:
- region: `nonwedge_intersection_chain`
- lane: `core_to_core_interface_strip`

Margin ordering on the strip:
- `weak_sector_anchor_sin2_theta_w = 0.4437`
- `weak_sector_volume_weighted_cross_ratio_exp01 = 0.3834`
- `e8_adjoint_cross_ratio_exp01 = 0.3502`
- `weak_sector_resonance_peak_exp02 = 0.3336`
- `weak_sector_resonance_band_mean_exp02 = 0.2931`

Interpretation:
Weak-style observables do not just "live on transitions" in a loose sense.
At current resolution they occupy one ordered interface strip with strong transport persistence.

### Promotion Boundary
Promoted from this ticket:
- weak-style observables currently track a stable interface-strip axis
- gauge weights remain ordered on one shared hosting spine

Not promoted:
- a full global symmetry-axis law for the jewel
- a clean interface-normal derivation
- any stronger claim that the hosting spine already resolves separate per-weight axes

### Best next use
Use this result for:
- bounded Level-1 writeup of hosting-axis structure
- future adjacency and connectivity interpretation
- later symmetry-probe refinement without reopening host-class questions


## 2026-03-15 - RFTP-1.45 Sector-Core / Transition-Surface Adjacency Graph

### Ticket
`RFTP-1.45 - Sector-Core / Transition-Surface Adjacency Graph`

### Objective
Build the first real connectivity graph of Level-1 geometry showing how stable sector cores, internal core submodes, transition surfaces, transition lanes, and mixed zones connect.

### Result
Classification: `partial_connectivity_graph_supported`

Bottom line:
The Level-1 map now has a usable connectivity graph.
It is not just a bag of labels.
The graph resolves into `19` nodes and `30` weighted edges, with strong internal core-core and lane-lane structure.
The wedge remains a dead-end mixed terminus, not a hosting hub.

### Main Findings

#### 1. The graph resolves clean object families and edge families
Counts:
- nodes: `19`
- edges: `30`
- strong edges: `22`

Edge classes:
- `core-core`: `14` edges, mean weight `0.9210`
- `core-lane`: `8` edges, mean weight `0.7112`
- `lane-lane`: `6` edges, mean weight `0.8432`
- `lane-mixed`: `2` edges, mean weight `0.9800`

Interpretation:
The strongest structure is still inside promoted object families, but the graph now also resolves real bridges from cores into lanes and from lanes into mixed termini.

#### 2. The main hosting routes are now explicit
Gauge-weight route:
- `central_hosting_spine -> core_to_core_interface_strip`
- strength `0.6606`

Weak-style route:
- `core_to_core_interface_strip -> bend_ridge -> mixed_wedge_terminus`
- strength `0.7764`

Interpretation:
The geometry/observable bridge can now be read as a route map rather than only as a host-class table.

#### 3. The most connected objects are meaningful geometric hubs
Main hubs:
- `fragility_shell_layer`
- `low_margin_shoulder`
- `bend_ridge`
- `collapse_core_subtype`
- `central_hosting_spine`

Interpretation:
The network is structured around stressed shell and transition objects, not around the wedge.
That supports a genuine Level-1 connectivity picture.

#### 4. Wedge placement stays bounded
`mixed_wedge_terminus` graph role:
- `dead_end`

`wedge_zone` remains:
- mixed
- attached only through the wedge terminus
- not a host hub

Interpretation:
Even after the graph construction, wedge stays a boundary terminus rather than a central organizing node.

### Promotion Boundary
Promoted from this ticket:
- Level-1 geometry has a real connectivity graph
- gauge and weak hosting routes can be stated in bounded route language
- wedge remains a mixed boundary terminus

Not promoted:
- a fully resolved global graph with bottlenecks or gateways locked
- any claim that every soft core-lane edge is equally stable

### Best next use
Use the graph for:
- symmetry-axis interpretation
- future Level-1 map summaries
- later adjacency refinement without changing the locked sector/transition taxonomy


## 2026-03-15 - RFTP-1.44 Transition Surface Internal Structure Mapping

### Ticket
`RFTP-1.44 - Transition Surface Internal Structure Mapping`

### Objective
Map the internal geometry of the locked transition surfaces and determine whether they are simple interfaces or structured manifolds with distinct internal lanes.

### Result
Classification: `weak_hosting_transition_lane_supported`

Bottom line:
The transition surfaces are structured, not simple interfaces.
They split into four readable lanes:
- `core_to_core_interface_strip`
- `bend_ridge`
- `low_margin_shoulder`
- `mixed_wedge_terminus`

The important new Level-1 result is that weak-style observables are not just transition-hosted in general.
They are concentrated on one specific transition lane:
`nonwedge_intersection_chain -> core_to_core_interface_strip`

### Main Findings

#### 1. The two promoted transition surfaces separate cleanly from the two mixed comparators
Promoted transition surfaces:
- `boundary_support_band`
- `nonwedge_intersection_chain`

Mixed low-margin comparators:
- `nonwedge_boundary_support_band`
- `wedge_zone`

Lane assignments:
- `boundary_support_band -> bend_ridge`
- `nonwedge_intersection_chain -> core_to_core_interface_strip`
- `nonwedge_boundary_support_band -> low_margin_shoulder`
- `wedge_zone -> mixed_wedge_terminus`

Interpretation:
Transition geometry is now first-class.
Mixed zones are not just weaker versions of the same object.

#### 2. Weak-style observables localize to one reproducible transition lane
Weak-style / transition-character candidates:
- `weak_sector_anchor_sin2_theta_w`
- `weak_sector_volume_weighted_cross_ratio_exp01`
- `e8_adjoint_cross_ratio_exp01`
- `weak_sector_resonance_band_mean_exp02`
- `weak_sector_resonance_peak_exp02`
- bounded extra companion: `su3_boundary_raw_invariant_exp05`

All of them currently host on:
- region: `nonwedge_intersection_chain`
- lane: `core_to_core_interface_strip`

Counts:
- weak host candidate count: `5`
- weak host lane count: `1`
- total transition-character hosts on that lane: `6`

Interpretation:
The weak-style hosting story is now sharper than “transition surface.”
At current resolution it is one nonwedge interface strip bridging overlap-fragility cores toward collapse geometry.

#### 3. Lane transport is strong
Mean lane transport rate:
- `0.9583`

Support-plane presence:
- `bend_ridge = 1.0000`
- `core_to_core_interface_strip = 1.0000`
- `low_margin_shoulder = 0.8889`
- `mixed_wedge_terminus = 0.0000`

Interpretation:
The lane map is not a one-slice artifact.
The high-transport object is the lane structure itself.

#### 4. Wedge stays excluded from promoted transition hosting
`wedge_zone` remained:
- `mixed_low_margin`
- lane: `mixed_wedge_terminus`
- weak host candidate count: `0`

Interpretation:
Even after opening the transition interiors, the wedge does not become the preferred host of weak-style observables.
That keeps the broader bridge clean.

### Promotion Boundary
Promoted from this ticket:
- transition surfaces have internal structure
- weak-style observables currently concentrate on a specific nonwedge transition lane

Not promoted:
- wedge as a transition host core
- mixed low-margin zones as true transition surfaces
- any broader claim that all transition-character observables must always live on exactly one lane beyond the current registry

### Best next use
Use the lane map for:
- `RFTP-1.45` adjacency graph construction
- core/transition connectivity work
- future geometry/observable bridge refinements


## 2026-03-15 - RFTP-1.43 Sector Core Geometry Characterization

### Ticket
`RFTP-1.43 - Sector Core Geometry Characterization`

### Objective
Resolve the internal geometry of the locked stable sector cores and determine whether they contain reproducible substructure relevant to hosted observables, especially the gauge-sector weights.

### Result
Classification: `gauge_weight_hosting_substructure_supported`

Bottom line:
The promoted sector cores are not just nonuniform in a generic way.
They now resolve into a specific hosting geometry:
- `central_hosting_spine`
- `outer_stable_shell`
- `fragility_shell_layer`
- `collapse_core_subtype`

The key upgrade over the earlier core-structure pass is that the gauge-sector weights now lock onto a distinct `central_hosting_spine` rather than merely a general low-risk core mode.

### Main Findings

#### 1. The stable sector cores split into four internal geometry submodes
Supported internal submodes:
- `central_hosting_spine`
  - region: `nonwedge_domain`
  - support compactness proxy: `0.5169`
  - mean support risk: `0.4831`
  - transport match rate: `1.0000`
- `outer_stable_shell`
  - region: `outer_anchor_shell`
  - support compactness proxy: `0.5887`
  - mean support risk: `0.4113`
  - transport match rate: `0.8182`
- `fragility_shell_layer`
  - regions: `inner_anchor_shell`, `overlap_tube`, `ridge_spine`
  - mean support risk: `0.6667`
  - mean failed rate: `0.4317`
  - transport match rate: `0.7576`
- `collapse_core_subtype`
  - regions: `intersection_chain`, `wedge_strip`
  - mean support risk: `0.7754`
  - mean failed rate: `0.5020`
  - transport match rate: `0.7727`

Interpretation:
The stable sector-core taxonomy now has a real internal geometry hierarchy rather than one flat core class.

#### 2. Gauge weights are now localized to one explicit hosting spine
Gauge-sector weights:
- `gauge_sector_weight_u1`
- `gauge_sector_weight_su2`
- `gauge_sector_weight_su3`

All three host on:
- region: `nonwedge_domain`
- geometry submode: `central_hosting_spine`
- core class: `overlap_fragility_curvature`

Lock metrics:
- gauge weight host region count: `1`
- central hosting spine region count: `1`
- gauge host density on that submode: `1.0`

Interpretation:
At current resolution the gauge-weight simplex does not split across multiple stable core pockets.
It lives on one common core-hosting spine.

#### 3. Transport is good enough to bank the internal core geometry
Mean transport match rate across the 7 stable cores:
- `0.8171`

Interpretation:
The new core-interior picture is not just a one-family readout.
The stable object is:
- one hosting spine
- one outer shell
- one overlap-fragility shell layer
- one collapse-core subtype

#### 4. The collapse-core subtype remains bounded
`intersection_chain` and `wedge_strip` remain a distinct stressed subtype:
- not the main gauge-weight host
- not a new hosting law
- still inside the promoted core taxonomy

Interpretation:
Failure-front-collapse hosting is still real, but still bounded.
It does not erase the simpler gauge-hosting picture.

### Promotion Boundary
Promoted from this ticket:
- stable sector cores contain reproducible internal geometry
- gauge weights currently localize to a distinct central hosting spine

Partial / bounded:
- outer stable shell as adjacent continuation of the hosting spine
- collapse-core subtype as a stressed core submode

Not promoted:
- separate per-weight subcores
- any claim of full internal symmetry reconstruction from the host spine alone

### Best next use
Use this result for:
- transition-vs-core comparison
- Level-1 adjacency mapping
- later symmetry-axis probing inside the stable core hosts

## 2026-03-14 - RFTP-1.44 Sector Core Structure Characterization

### Ticket
`RFTP-1.44 - Sector Core Structure Characterization`

### Objective
Map the internal structure of the sector-core regions that host the gauge-weight candidates.

### Result
Classification: `core_structure_submodes_supported`

Bottom line:
Sector cores are not homogeneous.
The current core map separates into three readable submodes:
- `weight_core_mode`
- `fragility_shell_mode`
- `collapse_core_subtype`

This is the first clear internal geometry result inside the promoted sector-core taxonomy.

### Main Findings

#### 1. Three core submodes are now supported
Supported core modes:
- `weight_core_mode`
  - regions: `nonwedge_domain`, `outer_anchor_shell`
  - mean failed rate: `0.2929`
  - mean support risk: `0.4472`
  - mean similarity margin: `0.1879`
- `fragility_shell_mode`
  - regions: `inner_anchor_shell`, `overlap_tube`, `ridge_spine`
  - mean failed rate: `0.4317`
  - mean support risk: `0.6667`
  - mean similarity margin: `0.1380`
- `collapse_core_subtype`
  - regions: `intersection_chain`, `wedge_strip`
  - mean failed rate: `0.5020`
  - mean support risk: `0.7754`
  - mean similarity margin: `0.1238`

Interpretation:
The stable core taxonomy now has internal regime structure, not just one undifferentiated host class.

#### 2. Gauge weights localize to one common low-risk core mode
Gauge-weight hosting:
- host region count: `1`
- shared host region: `nonwedge_domain`
- shared host mode: `weight_core_mode`
- shared host class: `overlap_fragility_curvature`

Weights:
- `U1 = 0.25`
- `SU2 = 0.30`
- `SU3 = 0.45`

Interpretation:
At current resolution, the gauge-weight simplex lives on a common stable weight-hosted core rather than on separate per-weight sub-cores.

#### 3. The overlap/fragility cores split into inner-shell stress and outer stable hosting
Lower-risk overlap/fragility layer:
- `nonwedge_domain`
- `outer_anchor_shell`

Higher-risk overlap/fragility shell:
- `inner_anchor_shell`
- `overlap_tube`
- `ridge_spine`

Interpretation:
The overlap/fragility class already contains a meaningful internal risk gradient.
That is exactly the kind of structure we want for later gauge-core interpretation work.

#### 4. Failure-front-collapse remains a distinct stressed subtype
Collapse subtype regions:
- `intersection_chain`
- `wedge_strip`

Current hosted observable:
- color resonance example

Interpretation:
The color-resonance bridge is now sitting on a genuine stressed core subtype, not just a one-off region label.

### Promotion Decision
Promote:
- sector-core internal submodes as a bounded geometry result
- `weight_core_mode` as the current common host layer for the gauge weights
- `collapse_core_subtype` as a stressed core subtype

Do not promote:
- separate per-weight host regions for `U1`, `SU2`, and `SU3`
- any direct physics-sector claim beyond current hosting geometry

### Best Next Step
Recommended next ticket: `gauge_weight_core_mode_writeup`

## 2026-03-14 - RFTP-1.43 Hosting Rule Broader Registry Monitoring

### Ticket
`RFTP-1.43 - Hosting Rule Broader Registry Monitoring`

### Objective
Continuously evaluate whether newly imported facet candidates continue to obey the locked `transition_character` hosting rule as the registry grows.

### Result
Classification: `rule_stable_under_registry_growth`

Bottom line:
The monitoring pass found no drift and no violations.
The locked hosting rule is fully stable under the current expanded registry snapshot.

Monitoring summary:
- registry candidates: `15`
- aligned candidates: `10`
- violations: `0`
- anomalies: `0`
- rule compliance rate: `1.0000`
- first deviation candidate: `none`

### Main Findings

#### 1. The current registry fully obeys the locked rule
Observed state:
- core-hosted share: `0.4`
- transition-hosted share: `0.6`
- mean alignment margin: `0.4341`

All three match the locked bridge baseline exactly.

Interpretation:
Registry growth has not yet introduced any candidate drift against the hosting rule.

#### 2. No wedge-like geometry drift is appearing through the back door
Monitoring status:
- every aligned candidate is `aligned_and_compliant`
- no rule-violation rows were generated
- first deviation remains `none`

Interpretation:
The rule is currently staying clean under actual registry monitoring, not just under synthetic perturbation tests.

#### 3. The monitor now gives explicit early-warning categories
Locked warning classes:
- `possible_candidate_error`
- `scale_caveat_issue`
- `taxonomy_update_candidate`
- `geometry_rule_violation`

Current run:
- none triggered

Interpretation:
The pipeline is now ready to flag future candidate drift without forcing an immediate taxonomy rewrite.

#### 4. Drift statistics are now baselined
Tracked metrics:
- registry size: `15`
- alignment-eligible count: `10`
- rule compliance rate: `1.0000`
- mean alignment margin: `0.4341`
- candidate class proportions: `0.4 / 0.6`

Interpretation:
Future candidate imports can now be judged against a locked bridge baseline instead of ad hoc memory.

### Promotion Decision
Promote:
- the monitoring pipeline
- the current conclusion that the rule remains stable under registry growth

Do not promote:
- any guarantee that future candidate imports cannot force revision

### Best Next Step
Recommended next ticket: `sector_core_structure_characterization`

## 2026-03-14 - RFTP-1.42 Hosting Rule Stress Test Under Candidate Perturbation

### Ticket
`RFTP-1.42 - Hosting Rule Stress Test Under Candidate Perturbation`

### Objective
Test whether the locked `transition_character` hosting rule survives realistic candidate-set perturbations, caveat filtering, and subtype regrouping.

### Result
Classification: `hosting_rule_robust_under_perturbation`

Bottom line:
The locked hosting rule did not just survive the perturbation pass.
It stayed exact across every tested slice.

Slice summary:
- tested slices: `10`
- robust slices: `10`
- minimum slice accuracy: `1.0000`
- minimum slice margin-weighted accuracy: `1.0000`
- sensitive caveat cases: `0`

### Main Findings

#### 1. The rule survives all candidate slices without qualitative change
Locked rule:
- `transition_character`

Passed slices:
- full aligned set
- verified synced only
- verified plus scale-caveated
- exclude provenance-limited
- exclude failure-front-collapse subtype
- exclude bounded-margin candidates
- gauge/weak only
- non-anchor additions only
- scale-caveated only
- duplicate-grouped weak resonance

Interpretation:
There is no sign here that the rule is an artifact of one narrow registry cut.

#### 2. Caveat filtering does not break the rule
Stable sensitivity cases:
- remove `su3_boundary_raw_invariant_exp05`
- remove `color_sector_killing_resonance_mean_exp04`
- remove `weak_sector_anchor_sin2_theta_w`
- remove all scale-caveated candidates
- remove all non-anchor additions

All cases:
- accuracy delta vs full: `0.0`
- sensitivity status: `stable`

Interpretation:
The rule does not depend on any one fragile candidate.

#### 3. Margin quality shifts, but not the rule itself
Examples:
- verified synced only mean margin: `0.6120`
- full aligned mean margin: `0.4341`
- non-anchor additions only mean margin: `0.3155`
- scale-caveated only mean margin: `0.3337`

Interpretation:
Some slices are cleaner than others, but none of them change the actual hosting split.

#### 4. Subtype regrouping does not change the outcome
Duplicate/subclass stress:
- collapsing the weak-resonance band/peak pair still keeps rule accuracy at `1.0000`
- removing the failure-front-collapse subtype still keeps rule accuracy at `1.0000`

Interpretation:
The current rule is not being propped up by duplicate handling or the color subtype.

### Promotion Decision
Promote:
- the hosting rule as robust under the current bounded perturbation suite

Do not promote:
- a universal claim beyond the current import protocol and registry family

### Best Next Step
Recommended next ticket: `hosting_rule_broader_registry_monitoring`

## 2026-03-14 - RFTP-1.41 Hosting Rule Writeup and Promotion Boundary Lock

### Ticket
`RFTP-1.41 - Hosting Rule Writeup and Promotion Boundary Lock`

### Objective
Freeze the hosting-rule result into manuscript-safe form with explicit promotion boundaries and candidate-side caveats.

### Result
Classification: `hosting_rule_writeup_confirmed`

Bottom line:
The hosting rule is now formally banked.
The canonical paper-safe wording is:

`Observables with strong transition character currently host on transition surfaces, while weight-like and static color-sector observables currently host on sector cores.`

This remains candidate-set bounded, but the rule itself is now clean enough to reuse.

### Main Findings

#### 1. The canonical rule is now locked
Locked rule:
- `transition_character`

Performance:
- evaluated aligned candidates: `10`
- best rule accuracy: `1.0000`
- best rule margin-weighted accuracy: `1.0000`

Interpretation:
The geometry-observable bridge now has a stable explanatory sentence, not just a table of alignments.

#### 2. Promotion boundaries are explicit
Promoted:
- the hosting rule itself
- core-hosted gauge weights
- transition-hosted weak-style observables

Partial:
- failure-front-collapse hosting as a bounded core subtype

Non-promoted:
- any universal or caveat-free hosting law
- any claim that candidate caveats no longer matter

Interpretation:
The writeup is now safer because the boundaries are explicit, not implied.

#### 3. Candidate-side caveats are now visible in the lock table
Counts:
- transition-character positive candidates: `6`
- scale-caveated candidates: `6`
- bounded-margin candidates: `1`

Representative examples:
- promoted core examples: the three gauge-sector weights
- promoted transition examples: weak anchor plus weak-style aligned additions
- bounded transition example: `su3_boundary_raw_invariant_exp05`
- partial subtype example: `color_sector_killing_resonance_mean_exp04`

Interpretation:
The rule is reusable, but only with the caveat labels preserved.

#### 4. Failure-front-collapse is now explicitly locked as subtype-only
Subtype lock:
- host subclass: `failure_front_collapse_core`
- strongest host region: `wedge_strip`
- margin: `0.3340`

Interpretation:
Color resonance currently supports a bounded core subtype note, not a third global hosting class.

### Promotion Decision
Promote:
- the hosting rule writeup
- the canonical transition-character wording
- the bounded geometry-observable bridge framing

Do not promote:
- any universal law claim beyond the current aligned set
- any independent global class for failure-front-collapse hosting

### Best Next Step
Recommended next ticket: `hosting_rule_stress_test_under_candidate_perturbation`

## 2026-03-14 - RFTP-1.40 Core-vs-Transition Hosting Rule Extraction

### Ticket
`RFTP-1.40 - Core-vs-Transition Hosting Rule Extraction`

### Objective
Extract the smallest structural rule that explains why some candidate observables align with stable sector cores while others align with transition surfaces.

### Result
Classification: `core_transition_hosting_rule_supported`

Bottom line:
The expanded bridge is no longer just an alignment fact.
It now admits a simple explanatory rule:
- observables with `transition_character` align with transition surfaces
- weight-like and static color-sector observables align with sector cores

Current bounded definition of `transition_character`:
- mixing/interpolation-sensitive
- or weak-sector running-sensitive

### Main Findings

#### 1. A one-feature rule separates all 10 aligned candidates
Best supported rule:
- `transition_character`

Definition:
- predict `transition_hosted` if the candidate is mixing/interpolation-sensitive or weak-sector running-sensitive
- otherwise predict `core_hosted`

Performance:
- evaluated candidates: `10`
- accuracy: `1.0000`
- margin-weighted accuracy: `1.0000`
- failures: `0`

Interpretation:
This is now the cleanest paper-safe explanation for the current bridge.

#### 2. The split is structurally sharp, not weakly suggestive
Specificity:
- `transition_character` transition-host rate: `1.0000`
- `transition_character` core-host rate: `0.0000`
- delta: `1.0000`

Related features:
- `mixing_like` delta: `0.8333`
- `running_sensitive` delta: `0.8333`
- `static_like` delta: `-1.0000`

Interpretation:
Transition hosting is currently tied to a coherent family of transition-sensitive observables, not to generic noise.

#### 3. Multiple simple proxy rules also fit, but are less canonical
Tied perfect rules:
- `static_like`
- `boundary_or_weak_scope`
- `scale_caveat`

Why `transition_character` is the right exported rule:
- it is the most geometry-facing and least registry-accidental wording
- it unifies weak mixing, weak resonance, and the bounded boundary-invariant case without reducing the split to a bookkeeping artifact

Interpretation:
The tie is useful, not a problem.
It says the current registry is internally consistent enough that several simple views recover the same split.

#### 4. Failure-front-collapse stays a bounded core subtype
Special-case check:
- `failure_front_collapse_core_rate` inside core-hosted set: `0.2500`

Interpretation:
The color-resonance placement currently reads as a bounded subtype of core hosting, not as a separate third hosting law.

### Promotion Decision
Promote:
- the bounded hosting rule: transition-character observables map to transition surfaces, while weight-like/static color-sector observables map to sector cores

Do not promote:
- a claim that the current rule is complete for all future observable families
- a standalone global hosting law for failure-front-collapse objects

### Best Next Step
Recommended next ticket: `hosting_rule_writeup`

## 2026-03-14 - RFTP-1.39 Expanded Candidate Bridge Writeup and Promotion Boundary Lock

### Ticket
`RFTP-1.39 - Expanded Candidate Bridge Writeup and Promotion Boundary Lock`

### Objective
Lock the expanded 10-candidate bridge into a manuscript-safe synthesis with explicit promotion boundaries, wedge exclusion, and candidate-type caveats.

### Result
Classification: `writeup_ready_with_candidate_caveats`

Bottom line:
The bridge is now broad enough to bank as a real writeup result.
The remaining limits are candidate caveats, not geometry instability.

Expanded bridge counts:
- eligible candidates: `10`
- core-aligned: `4`
- transition-aligned: `6`
- mixed: `0`
- inconclusive: `0`
- wedge-pull failures: `0`

### Main Findings

#### 1. The expanded bridge survives cleanly and strengthens
Bridge status:
- original 4-anchor bridge preserved: `true`
- mean alignment margin: `0.4341`
- gauge-weight core pattern supported: `true`
- weak-mixing transition pattern supported: `true`

Interpretation:
The bridge is now large enough to write up without pretending it is complete.

#### 2. Candidate-set caveats are now explicit rather than hidden
Aligned candidates:
- verified-strong: `3`
- scale-caveated: `6`
- provenance-limited aligned: `0`

Registry state:
- holdouts: `3`

Interpretation:
The current bridge is still bounded, but the limits are now named and quarantined instead of leaking into the geometry claim.

#### 3. Observable-class bridge wording is now lockable
Promoted writeup statements:
- gauge-sector weights are currently sector-core quantities
- weak-mixing-style observables are currently transition-surface quantities

Partial statements:
- color-resonance-style objects can live in failure-front-collapse cores
- the imported SU(3) boundary invariant remains transition-aligned

Non-promoted:
- complete facet census
- threshold-scale hosting claim
- wedge-zone hosting

Interpretation:
This is now the first manuscript-safe expanded geometry/physics bridge for the imported candidate registry.

#### 4. Wedge exclusion remains clean under expansion
Result:
- `0` wedge-pull failures
- minimum wedge gap: `0.1984`

Interpretation:
The expanded alignment still does not collapse into wedge attraction.
The canonical wedge zone remains excluded as a host core for the imported candidates.

### Promotion Decision
Promote:
- the expanded bridge as a stable geometry-class alignment result under the locked protocol
- gauge weights as currently core-hosted
- weak-mixing-style observables as currently transition-hosted

Do not promote:
- universal hosting claims beyond the current registry
- any threshold-scale interpretation
- any wedge-hosted facet interpretation

### Best Next Step
Recommended next ticket: `core_vs_transition_hosting_rule_extraction`

## 2026-03-14 - RFTP-1.38 Curvature-Mode Candidate Preference Analysis

### Ticket
`RFTP-1.38 - Curvature-Mode Candidate Preference Analysis`

### Objective
Test whether observable classes show systematic preference for the locked broader curvature classes once the candidate bridge is expanded beyond the original four Pioneer anchors.

### Result
Classification: `observable_class_curvature_bias_supported`

Bottom line:
Observable type now carries a real geometry-class bias.
The expanded candidate set preserves the original bridge and sharpens it into an observable-class split:
- gauge-weight observables are cleanly core-biased
- weak-mixing-style observables are cleanly transition-biased

This is now useful as a geometry-facing bridge result, but it is not yet a direct physics proof.

### Main Findings

#### 1. Gauge-weight observables are strongly core-hosted
Class:
- `gauge_coupling_weight`

Counts and preference:
- candidate count: `3`
- dominant mode: `overlap_fragility_core`
- mode preference rate: `1.0000`
- margin-weighted preference: `1.0000`
- mean core likelihood: `0.8742`

Members:
- `gauge_sector_weight_u1`
- `gauge_sector_weight_su2`
- `gauge_sector_weight_su3`

Interpretation:
The gauge-sector weights now behave like clean sector-core objects rather than transition or mixed-boundary quantities.

#### 2. Weak-mixing-style observables are transition-biased
Class:
- `weak_mixing_observable`

Counts and preference:
- candidate count: `5`
- dominant mode: `support_plane_bend_transition`
- mode preference rate: `1.0000`
- margin-weighted preference: `1.0000`
- mean transition likelihood: `0.4479`

Members:
- `weak_sector_anchor_sin2_theta_w`
- `weak_sector_volume_weighted_cross_ratio_exp01`
- `e8_adjoint_cross_ratio_exp01`
- `weak_sector_resonance_band_mean_exp02`
- `weak_sector_resonance_peak_exp02`

Interpretation:
The weak-sector lane is now behaving more like transition-surface geometry than sector-core geometry.
That is the first stable sign that different observable types may prefer different parts of the polytope map.

#### 3. Additional classes reinforce the split rather than weakening it
Single-candidate classes:
- `color_sector_resonance` -> dominant mode `failure_front_collapse_core`
- `boundary_invariant` -> dominant mode `support_plane_bend_transition`

Interpretation:
The non-gauge imports do not blur the picture.
They extend it:
- color-sector resonance currently reads as a collapse-core object
- the imported boundary invariant reads as transition geometry

#### 4. Threshold-scale observables remain unevaluated
Class:
- `threshold_scale`

Status:
- candidate count: `0`
- dominant mode preference: `not_evaluated_registry_limited`

Interpretation:
There is still no honest threshold-scale geometry claim to make from this registry version.
That stays a candidate-set limitation, not a negative result.

### Promotion Decision
Promote:
- observable-class curvature bias as a bounded bridge result
- gauge weights as core-biased within the current verified/import-cleared registry
- weak-mixing-style observables as transition-biased within the current verified/import-cleared registry

Do not promote:
- any direct physics claim beyond geometry-class preference
- any threshold-scale conclusion
- any claim that every future weak-sector observable must be transition-hosted

### Best Next Step
Recommended next ticket: `expanded_candidate_bridge_writeup`

## 2026-03-14 - RFTP-1.37 Expanded Candidate Alignment Sweep

### Ticket
`RFTP-1.37 - Expanded Candidate Alignment Sweep`

### Objective
Run the first full alignment sweep over the `10` alignment-eligible candidates using the locked sector/transition taxonomy and the 1.36 guardrails.

### Result
Classification: `core_transition_split_strengthened`

Bottom line:
The original bridge not only survives registry expansion, it strengthens under the larger candidate set.

With guardrails enforced:
- `4` candidates classify as `core_aligned_candidate`
- `6` classify as `transition_aligned_candidate`
- `0` classify as `mixed_boundary_candidate`
- `0` are `alignment_inconclusive`

No new region classes were needed, and no candidate was falsely pulled into the wedge zone.

### Main Findings

#### 1. The bridge survives expansion cleanly
Sweep totals:
- eligible candidates: `10`
- core-aligned: `4`
- transition-aligned: `6`
- mixed-boundary: `0`
- inconclusive: `0`

Guardrail outcomes:
- bridge preserved: `true`
- mean alignment margin: `0.4341`
- minimum wedge-pull gap: `0.1984`
- wedge-pull failures: `0`

Interpretation:
The core-vs-transition split now looks more robust than the original 4-anchor bridge, not less.

#### 2. Gauge-sector weights stay anchored in overlap/fragility sector cores
Candidates:
- `gauge_sector_weight_u1`
- `gauge_sector_weight_su2`
- `gauge_sector_weight_su3`

Classification:
- class: `core_aligned_candidate`
- strongest class: `overlap_fragility_core`
- strongest region: `nonwedge_domain`
- representative margin: `0.6681`

Interpretation:
The original gauge-sector bridge result remains completely stable under expansion.

#### 3. Weak-style observables remain transition-hosted
Candidates:
- `weak_sector_anchor_sin2_theta_w`
- `weak_sector_volume_weighted_cross_ratio_exp01`
- `e8_adjoint_cross_ratio_exp01`
- `weak_sector_resonance_band_mean_exp02`
- `weak_sector_resonance_peak_exp02`

Classification:
- class: `transition_aligned_candidate`
- strongest class: `transition_surface`
- strongest region: `nonwedge_intersection_chain`
- margins span `0.2931` to `0.4437`

Interpretation:
The weak-sector lane is no longer a one-off anchor effect.
It now behaves like a repeatable transition-surface preference pattern.

#### 4. New imports extend the taxonomy without forcing new geometry classes
Additional aligned candidates:
- `color_sector_killing_resonance_mean_exp04`
  - class: `core_aligned_candidate`
  - strongest class: `failure_front_collapse_core`
  - strongest region: `wedge_strip`
  - margin: `0.3340`
- `su3_boundary_raw_invariant_exp05`
  - class: `transition_aligned_candidate`
  - strongest class: `transition_surface`
  - strongest region: `nonwedge_intersection_chain`
  - margin: `0.1984`
  - strength: `bounded`

Interpretation:
The expanded sweep still lives entirely inside the locked taxonomy:
- overlap/fragility core
- failure-front-collapse core
- transition surface

No new ad hoc region class had to be invented to accommodate the extra candidates.

#### 5. Guardrails held under full sweep conditions
All `10` candidates:
- passed QC gating
- passed margin threshold review
- cleared the wedge guardrail

Locked duplicate handling applied to:
- `weak_sector_anchor_sin2_theta_w`
- the weak-resonance peak/band pair

Interpretation:
The expanded sweep looks trustworthy because the registry and alignment guardrails were actually exercised, not bypassed.

### Promotion Decision
Promote:
- the expanded bridge as stable under current registry expansion
- the core-vs-transition split as stronger than the original 4-anchor bridge

Do not promote:
- any claim that the current registry is complete
- any mixed-boundary interpretation, since none were needed here
- any weakening of the wedge exclusion rule

### Best Next Step
Recommended next ticket: `curvature_mode_candidate_preference_analysis`

## 2026-03-14 - RFTP-1.36 Expanded Candidate Alignment Readiness Audit

### Ticket
`RFTP-1.36 - Expanded Candidate Alignment Readiness Audit`

### Objective
Audit the locked sector/transition alignment pipeline so it can absorb a broader candidate registry without distorting the 1.34 bridge result.

### Result
Classification: `alignment_ready_with_guardrails`

Bottom line:
The alignment lane is ready for a larger registry, but only under explicit guardrails.

The geometry side did not need to change.
What changed was protocol hardening:
- duplicate handling is now explicit
- scale-caveat preservation is now explicit
- provenance-limited candidates are quarantined before scoring
- wedge-pull exclusion is now locked as a batch rule

### Main Findings

#### 1. Ten candidates are now eligible for bounded batch alignment
QC-cleared statuses:
- `ready_for_alignment`
- `needs_scale_caveat`

Counts:
- total candidates: `15`
- alignment-eligible after QC: `10`
- `ready_for_alignment`: `4`
- `needs_scale_caveat`: `6`
- `needs_better_provenance`: `2`
- `hold_out`: `3`

Interpretation:
The expanded registry is large enough for a real next alignment sweep, but not every imported entry should be scored yet.

#### 2. Duplicate handling is now locked
Covered groups:
- `weak_mixing_anchor_0217391`
  - action: collapse to `weak_sector_anchor_sin2_theta_w`
  - hold the demoted `5/23` duplicate out of scoring
- `weak_resonance_cluster_024x`
  - action: preserve the band-mean and peak as a linked pair
  - do not collapse them into one number prematurely

Interpretation:
The first likely large-registry failure mode is now addressed before it can blur the bridge result.

#### 3. Margin and wedge guardrails are now explicit
Locked thresholds:
- strong alignment margin: `>= 0.25`
- bounded alignment margin: `0.10 - 0.25`
- weak margin: `< 0.10` -> force `unresolved`
- clear wedge gap: `>= 0.10`
- wedge review band: `0.05 - 0.10`

Locked reference values from the current bridge:
- mean alignment margin: `0.5202`
- minimum wedge gap: `0.4437`

Interpretation:
The current bridge margins are comfortably above the new protocol floors, so the expanded sweep can proceed without relaxing the lock standards.

#### 4. Provenance quarantine is now a first-class rule
Candidates held out of alignment until provenance improves:
- `su3_boundary_invariant_02191_synthesis`
- `weinberg_threshold_mu_star_synthesis`

Interpretation:
Useful synthesis-only clues can stay in the registry without being mistaken for artifact-backed alignment inputs.

### Promotion Guidance

Promote:
- the claim that the alignment pipeline is ready for a larger registry under explicit guardrails
- the margin protocol
- duplicate handling
- wedge-pull guardrails

Do not promote:
- any claim that all expanded candidates are already alignment-safe
- any claim that provenance-limited synthesis entries can be scored like artifact-backed candidates

### Recommended Next Step
`expanded_candidate_alignment_sweep`

## 2026-03-14 - RFTP-1.35 Candidate Registry Expansion Under Locked Protocol

### Ticket
`RFTP-1.35 - Candidate Registry Expansion Under Locked Protocol`

### Objective
Expand the facet-candidate registry beyond the 4-anchor bridge while preserving the locked 1.34 import discipline and caveat handling.

### Result
Classification: `candidate_registry_expanded_with_holdouts`

Bottom line:
The registry expanded cleanly from `4` to `15` entries without changing the geometry taxonomy.

The expansion is useful and structured, but it is not flat:
- some candidates are ready
- some require scale-caveat preservation
- some need better provenance
- some are explicitly quarantined as holdouts

### Main Findings

#### 1. The expanded registry is now structured, not ad hoc
Registry composition:
- verified synced anchors: `4`
- artifact-backed exploratory candidates: `9`
- synthesis-note-only candidates: `2`

QC outcome:
- `ready_for_alignment`: `4`
- `needs_scale_caveat`: `6`
- `needs_better_provenance`: `2`
- `hold_out`: `3`

Interpretation:
The registry can now grow without blurring the boundary between trustworthy imports and exploratory or demoted material.

#### 2. The holdout set is clean and scientifically justified
Explicit holdouts:
- `color_sector_su3_boundary_echo_exp04`
- `casimir_dim_weighted_5_over_23_exp06`
- `casimir_alpha2_h_match_exp06`

Interpretation:
These are not missing-data accidents.
They are deliberate quarantines of candidates already debunked or demoted on the EXP side.

#### 3. Two synthesis-level candidates were admitted only as provenance-limited
Bounded candidates:
- `su3_boundary_invariant_02191_synthesis`
- `weinberg_threshold_mu_star_synthesis`

Interpretation:
These stay visible in the registry because they matter for future bridge work, but they are not yet artifact-backed enough for alignment scoring.

#### 4. The best artifact-backed additions are now locally available with clean provenance
Notable new artifact-backed entries:
- `weak_sector_volume_weighted_cross_ratio_exp01`
- `e8_adjoint_cross_ratio_exp01`
- `weak_sector_resonance_band_mean_exp02`
- `weak_sector_resonance_peak_exp02`
- `color_sector_killing_resonance_mean_exp04`
- `su3_boundary_raw_invariant_exp05`

Interpretation:
The next broader alignment sweep will no longer be limited to the 4 synced Pioneer anchors.

### Promotion Guidance

Promote:
- the expanded registry as a clean protocol object
- the QC split between ready, scale-caveated, provenance-limited, and holdout entries
- the explicit quarantine of demoted EXP candidates

Do not promote:
- any claim that the expanded registry is fully ready for alignment without guardrails
- any claim that synthesis-note-only entries are equivalent to raw artifact-backed candidates

### Recommended Next Step
`expanded_candidate_alignment_readiness_audit`

## 2026-03-14 - RFTP-1.34 Facet Candidate Bridge Writeup and Geometry-Class Lock

### Ticket
`RFTP-1.34 - Facet Candidate Bridge Writeup and Geometry-Class Lock`

### Objective
Lock the first manuscript-safe geometry-class bridge between the broader Codex taxonomy and the verified synced Pioneer facet anchors.

### Result
Classification: `core_transition_bridge_locked`

Bottom line:
The first narrow bridge is now locked cleanly:
- gauge-sector weights are `core-hosted facet candidates`
- the weak-sector anchor is a `transition-hosted candidate`
- no imported candidate is wedge-core aligned

This is a real bridge result, but it remains explicitly bounded to the current verified Pioneer sync set.

### Main Findings

#### 1. Gauge-sector weights are now locked as core-hosted candidates
Candidates:
- `gauge_sector_weight_u1`
- `gauge_sector_weight_su2`
- `gauge_sector_weight_su3`

Locked hosting class:
- `overlap_fragility_core`

Locked strongest region:
- `nonwedge_domain`

Numbers:
- mean alignment score: `0.8822`
- mean alignment margin: `0.5457`

Interpretation:
These imported gauge-sector simplex weights are now safely describable as core-hosted facet candidates under the locked broader taxonomy.

#### 2. The weak-sector anchor is now locked as transition-hosted
Candidate:
- `weak_sector_anchor_sin2_theta_w`

Locked hosting class:
- `transition_surface`

Locked strongest region:
- `nonwedge_intersection_chain`

Numbers:
- alignment score: `0.7311`
- alignment margin: `0.4437`

Interpretation:
The weak-sector anchor does not look like a stable sector-core host. It aligns more naturally with transition-surface geometry.

#### 3. The candidate-set boundary is explicit and important
Current imported registry:
- `4` verified synced Pioneer anchors only

Source:
- `polytope_global_targets.json`

Interpretation:
This bridge is real and usable, but it is not a complete facet census. It is a candidate-set-bounded lock, not a universal hosting map.

#### 4. Wedge exclusion stayed clean
For all imported candidates:
- `wedge_exclusion_status = pass`
- `wedge_pull_count = 0`

Interpretation:
The canonical wedge zone is not the host core for any currently imported verified candidate. It remains a mixed boundary object, not a facet-core fallback.

#### 5. A forward import protocol is now part of the lock
Future candidate imports should include:
- candidate name
- target descriptor
- value text
- provenance
- confidence level
- scale caveat if relevant

And most importantly:
- new candidates may be aligned against the locked taxonomy
- they may not rewrite the taxonomy without a separate geometry ticket

### Promotion Guidance

Promote:
- gauge-sector weights as core-hosted facet candidates
- weak-sector anchor as a transition-hosted candidate
- the explicit claim that no verified imported candidate prefers the mixed wedge zone

Promote only with caveat:
- the bridge is currently bounded to the verified Pioneer sync set
- this is geometry-hosting evidence, not physical confirmation
- weak-sector interpretation still carries RG-running / scale caveats

Do not promote:
- any claim that the current imported set is a full facet census
- any claim that the wedge zone hosts these candidates
- any claim that transition-hosted means physics-confirmed mixing origin

### Recommended Next Step
`expand_candidate_registry_under_locked_protocol`

## 2026-03-14 - RFTP-1.33 Sector/Transition Alignment with Facet Candidates

### Ticket
`RFTP-1.33 - Sector/Transition Alignment with Facet Candidates`

### Objective
Test whether the locked broader-polytope sector/transition taxonomy aligns in a stable and non-forced way with the current synced facet candidates from the other track.

### Result
Classification: `core_vs_transition_candidate_split_supported`

Bottom line:
The current frozen candidate set splits cleanly across the locked taxonomy:
- `3` candidates are strongly core-aligned
- `1` candidate is strongly transition-aligned
- `0` are mixed-boundary
- `0` are inconclusive
- `0` are falsely pulled into the wedge boundary

That is a meaningful bridge result.

### Import Boundary
Current candidate import was intentionally minimal and frozen:
- `gauge_sector_weight_u1`
- `gauge_sector_weight_su2`
- `gauge_sector_weight_su3`
- `weak_sector_anchor_sin2_theta_w`

Source:
- `polytope_global_targets.json`

Interpretation:
No richer synced facet-candidate registry was present locally, so this run stayed strictly inside the verified Pioneer sync objects.

### Main Findings

#### 1. Gauge-sector weights align strongly with stable sector cores
All three gauge-sector weight candidates aligned as:
- `core_aligned_candidate`

Strongest hosting class:
- `overlap_fragility_core`

Strongest region association:
- `nonwedge_domain`

Alignment numbers:
- score: `0.8822`
- margin over next-best class: `0.5457`
- wedge-pull gap: `0.8008`

Interpretation:
The current gauge-sector simplex weights look much more like stable sector-core objects than transition or wedge-boundary objects.

#### 2. The weak-sector anchor aligns with transition geometry
Candidate:
- `weak_sector_anchor_sin2_theta_w`

Alignment:
- `transition_aligned_candidate`

Strongest hosting class:
- `transition_surface`

Strongest region association:
- `nonwedge_intersection_chain`

Alignment numbers:
- score: `0.7311`
- margin over next-best class: `0.4437`
- second-best class: `mixed_low_margin`
- wedge-pull gap: `0.4437`

Interpretation:
The weak-sector anchor does not look best hosted by a stable core sector. It aligns more naturally with bend-associated transition geometry, which is exactly the kind of core-vs-transition split 1.33 was meant to test.

#### 3. The wedge-boundary sanity check passed cleanly
For all four candidates:
- `wedge_pull_flag = false`
- `sanity_result = clean`

Interpretation:
This matters a lot. The mixed wedge boundary is not just attracting nearby candidate alignments by geometric proximity. The split survives the explicit wedge-sanity check.

#### 4. The first useful core-vs-transition candidate taxonomy now exists
Locked split:
- Core-aligned candidates:
  - `gauge_sector_weight_u1`
  - `gauge_sector_weight_su2`
  - `gauge_sector_weight_su3`
- Transition-aligned candidate:
  - `weak_sector_anchor_sin2_theta_w`

Interpretation:
This is the first broader bridge result that cleanly separates likely sector-core targets from likely transition-associated targets.

### Promotion Guidance

Promote into the broader bridge story:
- gauge-sector simplex weights as core-aligned candidates
- weak-sector anchor as transition-aligned candidate
- the explicit claim that none of the current candidates are wedge-boundary dominated

Promote only with caveat:
- this alignment uses the current minimal synced candidate registry only
- alignment is geometric hosting evidence, not physics confirmation

Do not promote:
- direct proof that any candidate is the correct facet
- any claim that the wedge zone hosts a clean facet core
- any claim that transition alignment is equivalent to physical mixing confirmation

### Current Bridge Picture
- stable sector cores host the current gauge-sector weight candidates
- transition surfaces host the current weak-sector anchor candidate
- mixed wedge/boundary zones are not the preferred hosts of the current candidate set

### Recommendation For Next Step
Current recommended follow-on:
- `facet_candidate_bridge_writeup`

Reason:
- the candidate split is now strong enough to write up cleanly
- the next value is a bounded geometry/physics bridge note, not more alignment churn

### Artifacts
- Summary:
  - `results/20260314_220643_polytope_facet_alignment_v1_s20000_seed26/polytope_facet_alignment_summary.json`
- Main tables:
  - `results/20260314_220643_polytope_facet_alignment_v1_s20000_seed26/polytope_facet_candidate_import.csv`
  - `results/20260314_220643_polytope_facet_alignment_v1_s20000_seed26/polytope_facet_alignment_table.csv`
  - `results/20260314_220643_polytope_facet_alignment_v1_s20000_seed26/polytope_candidate_core_transition_taxonomy.csv`
  - `results/20260314_220643_polytope_facet_alignment_v1_s20000_seed26/polytope_wedge_alignment_sanity_check.csv`
- Bridge note:
  - `results/20260314_220643_polytope_facet_alignment_v1_s20000_seed26/polytope_facet_alignment_bridge_note.md`

### One-Sentence Research Memory
The 1.33 bridge lane found a clean split in the frozen candidate set: gauge-sector simplex weights are strongly core-aligned, the weak-sector anchor is strongly transition-aligned, and none of the current candidates are being falsely hosted by the mixed wedge boundary.

## 2026-03-14 - RFTP-1.32 Broader Polytope Curvature Writeup and Sector/Transition Taxonomy Lock

### Ticket
`RFTP-1.32 - Broader Polytope Curvature Writeup and Sector/Transition Taxonomy Lock`

### Objective
Synthesize the 1.31 broader-transfer result into a durable curvature-based taxonomy of stable sector cores, transition surfaces, mixed low-margin zones, and explicit non-core regions.

### Result
Classification: `sector_transition_taxonomy_locked`

Bottom line:
The broader polytope can now be described with a bounded curvature taxonomy:
- `7` surfaced regions lock as stable sector cores
- `2` lock as transition surfaces
- `2` lock as mixed low-margin zones
- `1` remains an aggregate reference, not a sector label

The broader map is now safe to use, with explicit caveats on transition geometry and wedge-like mixed zones.

### Main Findings

#### 1. Stable sector-core taxonomy is now explicit
Locked stable sector-core classes:
- `overlap_fragility_curvature`
  - representative regions:
    - `nonwedge_domain`
    - `inner_anchor_shell`
    - `outer_anchor_shell`
    - `overlap_tube`
    - `ridge_spine`
- `failure_front_collapse`
  - representative regions:
    - `intersection_chain`
    - `wedge_strip`

Interpretation:
These are now the two safe broader sector-core curvature descriptors. They can be reused in later mapping work as geometric labels, with the usual caution that they are not yet direct physics labels.

#### 2. Support-plane bend is locked as transition geometry only
Locked role:
- `support_plane_bend` -> `transition_surface`

Representative transition-associated regions:
- `boundary_support_band`
- `nonwedge_intersection_chain`
- `nonwedge_boundary_support_band`
- `wedge_zone`

Key evidence:
- bend presence rate across transition-associated regions: `0.7368`

Interpretation:
Support-plane bend is now safe to promote only as transition-surface geometry. It is not a stable sector-core label.

#### 3. Transition and mixed zones are now separated cleanly
Transition surfaces:
- `boundary_support_band`
- `nonwedge_intersection_chain`

Mixed low-margin zones:
- `nonwedge_boundary_support_band`
- `wedge_zone`

Interpretation:
This is important. Not everything outside the stable cores is the same object. Some regions are usable transition surfaces; some remain too mixed and low-margin to promote beyond boundary/mixing language.

#### 4. The canonical wedge zone now has final broader-map wording
Locked safe description:
- the canonical wedge zone is a `mixed low-margin transition-associated zone`
- it is useful as a `regime-mixing boundary object`
- it is not a stable sector core
- it is not a clean facet label
- it is not an exported support-plane-bend sector

Key evidence:
- dominant mode: `mixed_or_indeterminate`
- dominant consistency: `1.0000`
- mean similarity margin: `0.0226`
- mean failed rate: `0.5403`

Interpretation:
This closes the wedge-to-broader-map bridge in the safest possible way. The wedge zone belongs in the taxonomy as a mixed boundary region, not as a promoted sector.

#### 5. The broader writeup now has a reusable protocol
Locked protocol:
- stable sector-core classes can be reused as broader geometric labels
- transition-surface classes can be reused for boundary/interpolation studies
- mixed low-margin zones should not be sharpened without new evidence
- support-plane bend should remain transition-only unless stronger sector evidence appears
- residue is not part of the broader taxonomy object

Interpretation:
This is the handoff the rest of the polytope program needed. Future lanes now know what to reuse and what not to overclaim.

### Promotion Guidance

Promote into broader polytope mapping:
- `overlap_fragility_curvature` as a stable sector-core descriptor
- `failure_front_collapse` as a stable stressed sector-core descriptor
- `support_plane_bend` as a transition-surface descriptor only
- `mixed_or_indeterminate` as a non-core boundary/mixing label

Promote only with caveat:
- transition surfaces are first-class geometry objects, but they are not core sectors
- `wedge_strip` can be used as a stressed sector-core example, but should still be described as wedge-adjacent

Do not promote:
- direct physics meaning for any sector class yet
- the canonical wedge zone as a stable sector
- support-plane bend as a stable core class
- residue as part of the broader taxonomy

### Current Broader Polytope Map
- stable sector cores:
  - overlap / fragility sectors
  - failure-front collapse sectors
- transition surfaces:
  - bend-associated boundary/interpolation geometry
- mixed low-margin zones:
  - wedge-like or boundary-like mixing regions
- aggregate reference:
  - full canonical domain only

### Recommendation For Next Step
Current recommended follow-on:
- `sector_transition_alignment_with_facet_candidates`

Reason:
- the broader geometry taxonomy is now locked
- the highest-value next move is alignment and comparison, not more local classification churn

### Artifacts
- Summary:
  - `results/20260314_215646_polytope_curvature_writeup_v1_s20000_seed26/polytope_curvature_writeup_summary.json`
- Main tables:
  - `results/20260314_215646_polytope_curvature_writeup_v1_s20000_seed26/polytope_sector_transition_taxonomy.csv`
  - `results/20260314_215646_polytope_curvature_writeup_v1_s20000_seed26/polytope_region_classification_notes.csv`
  - `results/20260314_215646_polytope_curvature_writeup_v1_s20000_seed26/polytope_transition_structure_lock.csv`
  - `results/20260314_215646_polytope_curvature_writeup_v1_s20000_seed26/polytope_wedge_boundary_wording.csv`
- Writeup note:
  - `results/20260314_215646_polytope_curvature_writeup_v1_s20000_seed26/polytope_curvature_writeup_note.md`
- Figure caption:
  - `results/20260314_215646_polytope_curvature_writeup_v1_s20000_seed26/polytope_sector_transition_figure_caption.md`

### One-Sentence Research Memory
The 1.32 synthesis locked the broader polytope into a usable curvature taxonomy: overlap-fragility and failure-front-collapse are stable sector-core descriptors, support-plane bend is transition-only, and the canonical wedge zone is a mixed low-margin boundary object rather than a core sector.

## 2026-03-14 - RFTP-1.31 Curvature-Mode Transfer into Broader Polytope Mapping

### Ticket
`RFTP-1.31 - Curvature-Mode Transfer into Broader Polytope Mapping`

### Objective
Test whether the wedge-lane curvature modes can be exported into broader canonical polytope mapping as reusable geometric descriptors rather than staying wedge-only summaries.

### Result
Classification: `curvature_modes_transfer_supported`

Bottom line:
The wedge-lane curvature vocabulary does transfer beyond the original wedge analysis. It organizes broader canonical regions more coherently than the old threshold-style framing and better than axis-only ordering. But the transfer is not uniform across all three modes:
- overlap / fragility curvature exports cleanly as a stable sector-class signal
- failure-front collapse also exports cleanly in selected broader regions
- support-plane bend exports mainly as a transition-zone signature rather than a stable sector-core class

### Main Findings

#### 1. Broader transfer is real, not just wedge-local
Key evidence:
- stable region count: `8`
- nonwedge stable region count: `6`
- transition region count: `4`

Interpretation:
The curvature vocabulary is now useful outside the wedge lane itself. This is no longer just a local diagnostic language for wedge replay failures.

#### 2. Curvature-mode mapping improves broader organization
Proxy-dispersion coherence:
- threshold style: `0.3420`
- axis only: `0.3393`
- axis + curvature mode: `0.2808`

Dispersion gains:
- vs threshold: `+0.0611`
- vs axis only: `+0.0585`

Interpretation:
Using the transferred curvature vocabulary organizes broader canonical regions substantially better than the earlier threshold framing and materially better than portable-axis ordering alone.

#### 3. Stable sector-like classes emerge outside the original wedge focus
Stable exported regions:
- `nonwedge_domain` -> `overlap_fragility_curvature`, consistency `1.0000`
- `outer_anchor_shell` -> `overlap_fragility_curvature`, consistency `0.8182`
- `inner_anchor_shell` -> `overlap_fragility_curvature`, consistency `0.7273`
- `overlap_tube` -> `overlap_fragility_curvature`, consistency `0.8182`
- `ridge_spine` -> `overlap_fragility_curvature`, consistency `0.7273`
- `intersection_chain` -> `failure_front_collapse`, consistency `0.7273`
- `wedge_strip` -> `failure_front_collapse`, consistency `0.8182`

Interpretation:
The exported vocabulary now has stable region-class behavior. Overlap/fragility looks like the dominant broader stable class, while failure-front collapse appears in sharper stressed subregions.

#### 4. Support-plane bend transfers mainly as transition geometry
Important nuance:
- `wedge_zone` remained fully `mixed_or_indeterminate` with mean similarity margin only `0.0226`
- `boundary_support_band` and `nonwedge_boundary_support_band` showed mode-flip or mixed-signature behavior

Interpretation:
Support-plane bend did not become a clean broad sector label. Instead it behaves more like a transition-surface vocabulary that helps identify where region classes mix or flip.

#### 5. The bridge to broader polytope mapping is now usable but still bounded
Paper-safe bridge note:
- low-failure stable nonwedge regions are the best candidates for future facet-core comparison
- support-plane-bend-dominant or mixed regions should be treated as transition-organizing zones, not settled sector cores
- collapse/fragility-dominant regions look boundary-stressed or failure-like, not symmetry-core-like

Interpretation:
This is the first wedge export that looks genuinely useful to the broader polytope program without forcing residue or threshold machinery into places they do not belong.

### Promotion Guidance

Promote into broader geometry work:
- the wedge curvature vocabulary as a reusable mapping language
- overlap / fragility curvature as a broader stable sector-class descriptor
- failure-front collapse as a broader stressed-region descriptor
- support-plane bend as a transition-zone / mixing-surface descriptor

Promote only with caveat:
- direct sector-class transfer should stay within canonical-family mapping for now
- support-plane bend should be described as transition-organizing, not as a settled stable class

Do not promote:
- direct physics-sector identification from curvature classes
- residue as part of the transfer object
- wedge-only threshold stories as the broader mapping language

### Current Broader Geometry Hierarchy
- portable axis = global compact-validity ordering
- branch map = wedge-lane regime structure
- curvature vocabulary = exported broader mapping language
- overlap / fragility curvature = stable sector-class descriptor
- failure-front collapse = stable stressed-region descriptor
- support-plane bend = transition-surface descriptor
- residue = not part of the transferable geometric mechanism

### Recommendation For Next Step
Current recommended follow-on:
- `broader_polytope_curvature_writeup`

Reason:
- the curvature export is now strong enough to serve as an input to broader polytope mapping
- the biggest new value is organizing sectors and transition zones, not reopening wedge-local searches

### Artifacts
- Summary:
  - `results/20260314_214641_polytope_curvature_transfer_v1_s20000_seed26/polytope_curvature_transfer_summary.json`
- Main tables:
  - `results/20260314_214641_polytope_curvature_transfer_v1_s20000_seed26/wedge_curvature_mode_export.csv`
  - `results/20260314_214641_polytope_curvature_transfer_v1_s20000_seed26/polytope_curvature_mode_transfer.csv`
  - `results/20260314_214641_polytope_curvature_transfer_v1_s20000_seed26/polytope_curvature_sector_classes.csv`
  - `results/20260314_214641_polytope_curvature_transfer_v1_s20000_seed26/polytope_transition_zone_map.csv`
- Bridge note:
  - `results/20260314_214641_polytope_curvature_transfer_v1_s20000_seed26/polytope_curvature_bridge_note.md`

### One-Sentence Research Memory
The 1.31 transfer lane showed that the wedge program exported a real broader curvature vocabulary: overlap/fragility and failure-front collapse became stable region-class descriptors, while support-plane bend exported mainly as a transition-zone signature rather than a stable sector label.

## 2026-03-14 - RFTP-1.30 Curvature Mode Writeup and Promotion Boundary Lock

### Ticket
`RFTP-1.30 - Curvature Mode Writeup and Promotion Boundary Lock`

### Objective
Convert the 1.21–1.29 wedge lane into a bounded paper-safe synthesis that promotes the stable geometric results and explicitly locks the non-promoted parts.

### Result
Classification: `writeup_ready_with_local_locks`

Bottom line:
The wedge lane is now bankable as a bounded geometric result. Two objects promote cleanly:
- the portable support-risk axis
- the multi-branch regime map

Four objects remain partial:
- the threshold gate
- the branch map as an operational policy
- the branch curvature backbone
- the anchor microregime as a local note

Three objects are now explicitly locked as non-promoted:
- the boundary-only residue law hypothesis
- residue as a governing law
- the anchor microregime as a portable rule or shoulder law

### Main Findings

#### 1. The portable axis is promoted as the global ordering object
Key evidence:
- mixed macro recall: `0.5333`
- failed-rate monotonicity: `0.7300`
- high-risk wedge enrichment: `1.5334`

Interpretation:
The portable support-risk axis is now the correct global compact-validity ordering coordinate for the wedge lane. The thresholds on it remain heuristic, but the axis itself is not in doubt.

#### 2. The branch map is promoted as the regime structure
Key evidence:
- mean boundary-robustness delta: `0.0216`
- branch-map Brier gain vs threshold: `+0.00239`
- branch-map calibration gain vs threshold: `+0.00813`

Interpretation:
The branch map is now the right regime object layered on the portable axis, even though it is still only a partial operational policy.

#### 3. The branch map has a real curvature backbone
Key evidence:
- all strong mode count: `6`
- portable mode proxy count: `6`
- mean transport consistency: `0.9333`

Canonical curvature hierarchy:
- early branch: `mixed overlap-collapse curvature mode`
- mid/late branch: `support-plane bend mode`
- late branch: `failure-front curvature mode`

Interpretation:
This is the main geometric upgrade of the wedge lane. The branch structure is not just predictive partitioning anymore; it has a stable curvature-like interpretation.

#### 4. Residue is now explicitly locked as non-governing
Key evidence:
- support-beats-residue rate: `1.0`
- combined-nonpositive rate: `1.0`

Interpretation:
Residue does not become a second law anywhere in the wedge lane. The safe promoted statement is negative: it is not governing, not global, and not the geometric quantity behind the branch map.

#### 5. The anchor microregime is locked as local-only
Key evidence:
- anchor-like gain: `+0.27001`
- wedge-like gain: `-0.28967`
- wedge-matched gain: `-0.32894`
- shape: `fuzzy_band`
- ordering: `with_support_collapse`
- anchor shoulder near-rate: `0.0`

Interpretation:
The anchor microregime remains worth mentioning, but only as a bounded anchor-enhanced fuzzy note. It is not portable, not leading, and not a crisp curvature shoulder.

### Promotion Guidance

Promote into main paper:
- `slice_percentile_pair_max` as the global compact-validity ordering coordinate
- the multi-branch regime map as the wedge-lane regime structure
- the partial curvature hierarchy of the branches:
  - early = overlap / fragility curvature
  - mid/late = support-plane bend
  - late = failure-front collapse

Promote only with explicit caveat:
- threshold gate as trust ordering, not final universal boundary
- branch map as a partial operational policy only
- curvature backbone as a partial geometry interpretation, not a solved manifold law
- anchor microregime only as a bounded local note

Do not promote:
- boundary-only residue law hypothesis
- residue as a global or governing law
- anchor microregime as a portable rule
- anchor microregime as a crisp curvature shoulder

### Final Wedge-Lane Hierarchy
- portable axis = global compact-validity ordering
- branch map = regime structure on that axis
- support geometry = governing mechanism
- curvature modes = partial geometric backbone of the regime structure
- residue = non-governing local companion only
- anchor microregime = local fuzzy nuance, not portable law

### Recommendation For Next Step
Current recommended follow-on:
- `use_curvature_modes_in_broader_polytope_mapping`

Reason:
- the wedge lane is mature enough to bank
- the main stable export is the axis + branch map + curvature backbone
- further residue mining is now lower-value than using these geometric objects in broader polytope work

### Artifacts
- Summary:
  - `results/20260314_212700_wedge_curvature_writeup_v1_s20000_seed26/wedge_curvature_writeup_summary.json`
- Main tables:
  - `results/20260314_212700_wedge_curvature_writeup_v1_s20000_seed26/wedge_promotion_boundary_table.csv`
  - `results/20260314_212700_wedge_curvature_writeup_v1_s20000_seed26/wedge_curvature_hierarchy_summary.csv`
  - `results/20260314_212700_wedge_curvature_writeup_v1_s20000_seed26/wedge_residue_role_lock.csv`
  - `results/20260314_212700_wedge_curvature_writeup_v1_s20000_seed26/wedge_anchor_microregime_nonpromotion.csv`
- Writeup note:
  - `results/20260314_212700_wedge_curvature_writeup_v1_s20000_seed26/wedge_curvature_writeup_note.md`
- Figure caption:
  - `results/20260314_212700_wedge_curvature_writeup_v1_s20000_seed26/wedge_lane_figure_caption.md`

### One-Sentence Research Memory
The 1.30 synthesis locked the wedge lane as a portable ordering axis plus multi-branch regime structure with a real but partial curvature backbone, while explicitly non-promoting residue and the anchor microregime beyond bounded local roles.

## 2026-03-14 - RFTP-1.29 Curvature Mode Identification

### Ticket
`RFTP-1.29 - Curvature Mode Identification`

### Objective
Determine whether the locked branch structure and anchor-enhanced microregime correspond to distinct curvature-like modes of the underlying support geometry, rather than only empirical predictive partitions.

### Result
Classification: `branch_curvature_structure_partial`

Bottom line:
The portable-axis branch map now has a real curvature-like geometric backbone. The early branch, mid/late branch, and late branch are not just statistical bins; they separate cleanly under a small interpretable proxy family. But the anchor microregime still does not sit tightly enough on one reproducible shoulder to justify a single clean curvature-shoulder claim.

### Main Findings

#### 1. Branch structure is visibly curvature-organized
Strong mode count:
- `all`: `6`
- `anchor_like`: `6`

Anchor-like branch phrases:
- early branch: `mixed overlap-collapse curvature mode`
- mid/late branch: `support-plane bend mode`
- late branch: `failure-front curvature mode`

Interpretation:
This is the first real geometry-level step beyond the predictive branch map. The three regimes behave like different curvature families of the same support object.

#### 2. The most portable curvature splits are very stable
Portable-mode proxy count: `6`

Mean transport consistency:
- `0.9333`

Proxy-level transport:
- `boundary_curvature_abs_mean` consensus: `early_wedge_fragility_branch`
- `intersection_curvature_abs_mean` consensus: `early_wedge_fragility_branch`
- `overlap_curvature_abs_mean` consensus: `early_wedge_fragility_branch`
- `failure_curvature_abs_mean` consensus: `midlate_wedge_support_branch`
- `support_plane_bend_mean` consensus: `midlate_wedge_support_branch`

Interpretation:
The curvature story is more portable than the earlier threshold gate story. What transports is not a hard boundary, but a stable ranking of which curvature mode dominates which regime family.

#### 3. The mid/late branch really does look bend-like
All-group mid/late proxy strengths:
- failure curvature: `3.2969`
- support-plane bend: `15.2880`

Anchor-like mid/late proxy strengths:
- failure curvature: `3.1524`
- support-plane bend: `5.6991`

Interpretation:
The mid/late wedge support-collapse branch is not best described as a simple boundary spike. It behaves more like a support-plane bend / mixed turning regime.

#### 4. The early branch stays structurally distinct
All-group early proxy strengths:
- boundary curvature: `1.4181`
- overlap curvature: `3.1779`

Anchor-like early proxy strengths:
- boundary curvature: `0.7757`
- overlap curvature: `1.9796`
- support-fragility curvature: `2.0769`

Interpretation:
The early wedge fragility branch remains a distinct local mode, not just a weak prelude to the later support-collapse regime.

#### 5. The anchor microregime does not lock to one clean shoulder
Best anchor shoulder proxy:
- `support_plane_bend_mean`

But:
- shoulder delta mean: `+0.0636`
- near-shoulder rate: `0.0`

Interpretation:
There is local geometric structure under the anchor pocket, but it is too fuzzy and slice-variable to promote as a single crisp curvature shoulder.

#### 6. Residue still looks companion-like relative to curvature stress
Anchor-like mid/late residue correlations:
- residue vs failure-curvature stress: `-0.2800`
- residue vs support-plane bend: `+0.0514`

Interpretation:
Residue does not emerge here as an independent geometric mode. At best it weakly tracks local bend stress, which fits the current “companion, not governing law” interpretation.

### Scientific Interpretation
- portable axis = global compact-validity ordering
- branch map = empirical regime structure
- curvature proxies = partial geometric explanation of that regime structure
- early branch = overlap / fragility heavy curvature mode
- mid/late branch = support-plane bend mode
- late branch = failure-front collapse mode
- anchor microregime = real local nuance, but not a clean portable curvature shoulder
- residue = bounded companion to local stress, not a governing mode

### Promotion Guidance

Promote into main paper:
- the claim that the branch map has a real curvature-like backbone
- the distinction between early fragility, mid/late bend, and late collapse modes
- the continued hierarchy that support geometry governs while residue remains bounded and auxiliary

Do not promote as established:
- a single sharp curvature shoulder under the anchor microregime
- any portable residue-curvature micro-law
- any statement that the anchor fuzzy band is now geometrically solved

Possible paper-safe framing:
- “The portable support-risk axis is not merely predictive: its branch structure aligns with distinct curvature-like modes of support geometry, while the anchor-local residue pocket remains a bounded fuzzy companion region rather than a portable geometric law.”

### Recommendation For Next Step
Current recommended follow-on:
- `curvature_mode_writeup_partial`

Reason:
- the branch geometry is now strong enough to bank
- the main remaining limit is the anchor microregime, which still fails to collapse into one clean portable shoulder

### Artifacts
- Summary:
  - `results/20260314_211652_wedge_curvature_modes_v1_s20000_seed26/wedge_curvature_synthesis_summary.json`
- Main tables:
  - `results/20260314_211652_wedge_curvature_modes_v1_s20000_seed26/wedge_curvature_mode_proxies.csv`
  - `results/20260314_211652_wedge_curvature_modes_v1_s20000_seed26/wedge_branch_curvature_profiles.csv`
  - `results/20260314_211652_wedge_curvature_modes_v1_s20000_seed26/wedge_anchor_curvature_shoulder.csv`
  - `results/20260314_211652_wedge_curvature_modes_v1_s20000_seed26/wedge_curvature_transport.csv`

### One-Sentence Research Memory
The 1.29 lane showed that the portable branch map is underwritten by distinct curvature-like support modes, but the anchor microregime still remains a fuzzy local nuance rather than a clean portable curvature shoulder.

## 2026-03-14 - RFTP-1.28 Anchor Microregime Note and Non-Transport Lock

### Ticket
`RFTP-1.28 - Anchor Microregime Note and Non-Transport Lock`

### Objective
Formally confirm, bound, and close the claim that the mid/late auxiliary pocket is an anchor-enhanced local microregime, not a portable residue micro-law.

### Result
Classification: `anchor_microregime_note_confirmed`

Bottom line:
The residue-helping pocket is real, but only as an anchor-enhanced fuzzy microregime inside the mid/late wedge support-collapse branch. It does not transport outside anchor-like slices, and it does not support precursor-law language. The safe final statement is:
- the pocket exists
- it is local
- it is fuzzy, not sharply bounded
- it is companion-like, not leading
- it should not be exported as a rule

### Main Findings

#### 1. The anchor microregime is real
Frozen minimal rule:
- `mid/late branch AND boundary_depth__mid AND anchor_like family`

Anchor-like transport lock:
- support-only AUROC: `0.48371`
- support-plus-residue AUROC: `0.75372`
- combined-vs-support gain: `+0.27001`
- sign consistency: `1.0`

Interpretation:
Inside anchor-like slices, the microregime is not ambiguous. The local auxiliary effect is large and stable enough to bank as a real local note.

#### 2. The same pocket fails to transport
Wedge-like:
- combined-vs-support gain: `-0.28967`
- sign consistency: `1.0`
- dominant relation: `after_support_collapse`

Wedge-matched:
- combined-vs-support gain: `-0.32894`
- sign consistency: `1.0`
- dominant relation: `after_support_collapse`

Interpretation:
This locks the non-transport result. The very same `boundary_depth__mid` pocket that helps anchor-like slices is harmful in the wedge families. That closes the door on any portable residue micro-law claim.

#### 3. The geometry is fuzzy-band, not a sharp pocket
Frozen geometry note:
- shape hint: `fuzzy_band`
- active cell count: `4 / 9`
- active cells:
  - `low:low`
  - `mid:low`
  - `high:mid`
  - `high:high`

Anchor core means:
- branch depth: `0.41362`
- support risk: `0.63791`
- boundary depth: `0.43050`
- intersection-rank mean: `0.40156`
- shared-overlap distance: `1.43678`

Interpretation:
The helpful region is not an isolated island. It is a fuzzy anchor-conditioned band spread across several local cells inside the mid/late branch.

#### 4. The pocket differs from neighbors mostly by position and overlap support
Anchor pocket vs adjacent neighbors:
- branch-depth delta: `-0.16556`
- support-risk delta: `-0.02318`
- intersection-rank delta: `-0.03404`
- shared-overlap-distance delta: `-0.02997`
- support-fragility delta: `+0.00268`

Interpretation:
The pocket is mostly a slightly earlier, tighter-overlap microstructure rather than a region with dramatically different support-fragility.

#### 5. This is companion-like, not early-warning
Anchor ordering lock:
- dominant relation: `with_support_collapse`
- residue-vs-support centroid delta: `+0.01639`
- early-warning supported: `False`

All-family ordering lock:
- dominant relation: `with_support_collapse`

Interpretation:
Residue does not lead support collapse in the anchor microregime. It tracks with it. So the correct language is “local companion marker,” not “local precursor law.”

#### 6. Global hierarchy remains unchanged
Global failure Brier:
- support-only: `0.22274`
- branch-local auxiliary: `0.22463`
- support-plus-residue: `0.24537`

Locked hierarchy:
- portable axis = global ordering object
- branch map = regime structure
- support geometry = governing mechanism
- anchor microregime = local companion-only nuance
- residue remains non-promoted globally

Interpretation:
This local note does not alter the promoted global mechanism picture.

### Promote / Do Not Promote

Promote:
- the existence of an anchor-enhanced fuzzy microregime inside the mid/late wedge support-collapse branch
- the minimal local rule:
  - `mid/late branch AND boundary_depth__mid AND anchor_like family`
- the statement that residue is companion-like there, not leading

Do not promote:
- any portable residue micro-law claim
- any early-warning or precursor-law phrasing
- any export of this pocket beyond anchor-like slices
- any reinterpretation of residue as a governing mechanism

### Current paper-safe interpretation
- portable axis = global compact-validity ordering
- branch map = regime structure on that axis
- support geometry = governing mechanism
- anchor microregime = fuzzy anchor-enhanced local nuance
- residue = local companion only, not portable, not governing, not promoted

### Recommended next step
`curvature_mode_identification`

## 2026-03-14 - RFTP-1.27 Mid/Late Auxiliary Subregion Geometry Audit

### Ticket
`RFTP-1.27 - Mid/Late Auxiliary Subregion Geometry Audit`

### Objective
Resolve the geometric structure of the bounded mid/late auxiliary pocket from 1.26 and determine whether it corresponds to a reproducible micro-regime on the portable support-risk axis with distinct support or boundary geometry.

### Result
Classification: `anchor_enhanced_microregime_supported`

Bottom line:
The auxiliary pocket survives the geometry audit, but it does not sharpen into a clean portable micro-law. The best pocket is still the simple `boundary_depth__mid` slice inside the mid/late branch. That pocket is strongly positive in anchor-like slices and strongly negative in wedge-like slices, so the safe interpretation is:
- the pocket is structurally real
- it is anchor-enhanced rather than broadly portable
- residue remains a local companion signal, not a governing law

### Main Findings

#### 1. The strongest pocket stayed simple
Selected pocket:
- `boundary_depth__mid`

Anchor-like performance:
- support-only AUROC: `0.48371`
- support-plus-residue AUROC: `0.75372`
- combined-vs-support gain: `+0.27001`
- positive gain rate: `1.0`

Interpretation:
The geometry audit did not uncover a narrower two-feature winner that displaced the 1.26 clue. The strongest stable pocket is still the mid boundary-depth slice itself.

#### 2. The pocket is clearly anchor-enhanced, not portable
Pocket gain by family:
- anchor-like: `+0.27001`
- all families: `+0.06013`
- wedge-like: `-0.28967`
- wedge-matched: `-0.32894`

Interpretation:
This is not a transport-stable residue micro-law. The same local pocket that helps the anchor-like families hurts the wedge-matched family.

#### 3. The pocket differs from nearby states mainly by position, not by a dramatic support-collapse jump
Anchor-like pocket vs adjacent neighbors:
- branch-depth delta: `-0.16556`
- support-risk delta: `-0.02318`
- boundary-depth delta: `+0.00877`
- intersection-rank delta: `-0.03404`
- shared-overlap-distance delta: `-0.02997`
- support-fragility delta: `+0.00268`

Interpretation:
The pocket looks like a slightly earlier, more overlap-supported position inside the mid/late branch, not a region with a dramatically different support-fragility level. The strongest contrast is positional along branch depth plus somewhat tighter overlap geometry.

#### 4. The helpful structure is broader than a single sharp cell
Anchor-like active cells in the `boundary_depth x branch_depth` grid:
- `low x low`
- `mid x low`
- `high x mid`
- `high x high`

Shape hint from the audit:
- `fuzzy_band`

Interpretation:
This is not a compact island. It looks more like an anchor-specific banded microstructure spread across a few locally favorable cells.

#### 5. Residue is not late here, but it is not clearly pre-collapse either
Anchor-like pocket ordering:
- dominant relation: `with_support_collapse`
- residue-vs-support centroid delta: `+0.01639`

Wedge-like pocket ordering:
- dominant relation: `after_support_collapse`
- residue-vs-support centroid delta: `+0.22669`

Interpretation:
Inside the anchor-like pocket, residue tracks support collapse almost simultaneously. In the wedge-like families it shifts later and becomes more obviously symptom-like.

#### 6. This did not support a transition-shoulder claim
Anchor-like pocket depth centroid:
- `0.41362`

Anchor-like peak failure-slope depth:
- `0.08333`

Pocket-to-peak slope delta:
- `+0.33028`

Interpretation:
The pocket does not sit on the main local failure shoulder of the anchor-like depth curve. That is why this ticket did not promote to `transition_shoulder_microregime_supported`.

### Promote / Do Not Promote

Promote:
- the existence of an anchor-enhanced auxiliary pocket inside the mid/late wedge support-collapse branch
- the fact that the best pocket is still keyed by `boundary_depth mid`
- the interpretation that residue can track a local anchor-specific microstructure without becoming a second law

Do not promote:
- any claim that this pocket is portable across slice families
- any claim that the pocket is a sharp isolated island or a universal transition shoulder
- any new residue-centered law language

### Current paper-safe interpretation
- portable axis = global compact-validity ordering
- branch map = regime structure on that axis
- support geometry = governing mechanism
- residue = local companion marker only in a bounded, anchor-enhanced mid/late microstructure

### Recommended next step
`anchor_microregime_note`

## 2026-03-14 - RFTP-1.26 Mid/Late Branch Auxiliary Role Confirmation Note

### Ticket
`RFTP-1.26 - Mid/Late Branch Auxiliary Role Confirmation Note`

### Objective
Confirm and bound the claim that wedge residue has a strictly local auxiliary role inside the mid/late wedge support-collapse branch, while remaining non-promotable globally and non-helpful in the early and late branches.

### Fixed ingredients
- Canonical fixture: `repaired_anchor_canonical_v1`
- Frozen portable axis:
  - `slice_percentile_pair_max`
- Frozen best refined branch map from 1.25:
  - early wedge fragility `0.00-0.17`
  - mid/late wedge support-collapse `0.58-0.72`
  - late full-anchor support-collapse core `0.72-0.88`
- Comparisons:
  - support-only
  - residue-only
  - support-plus-residue
- Global lock check:
  - support-only global policy
  - support-plus-residue global policy
  - branch-local auxiliary policy

### Result
Classification: `midlate_auxiliary_subregion_only`

Bottom line:
The mid/late branch residue signal survives, but it is narrower than a whole-branch rule. The safe statement is:
- residue has real auxiliary value in the mid/late branch
- that value is strongest in a specific subregion
- early branch is still clearly harmed by residue
- late anchor branch is still harmed in the anchor-like slices
- support-only remains the correct globally promoted mechanism

### Main Findings

#### 1. The mid/late branch benefit is real in anchor-like slices
Anchor-like mid/late branch:
- combined-vs-support AUROC gain mean: `+0.18756`
- positive gain rate: `1.0`
- positive gain rate above `0.02`: `1.0`

Interpretation:
Inside the canonical anchor-like replay context, the mid/late branch auxiliary effect is not fragile. It replicates cleanly.

#### 2. The same effect does not generalize to all families
All-family mid/late branch:
- combined-vs-support gain mean: `+0.01824`

Wedge-like mid/late branch:
- combined-vs-support gain mean: `-0.06814`

Control mid/late branch:
- combined-vs-support gain mean: `-0.23232`

Interpretation:
This is not a universal branch law. It is an anchor-like local utility effect, not a transport-invariant residue rule.

#### 3. Early and late branches still reject residue
Early branch, all slices:
- combined-vs-support gain mean: `-0.24202`
- negative gain rate: `1.0`

Late branch, anchor-like slices:
- combined-vs-support gain mean: `-0.05409`
- negative gain rate: `1.0`

Interpretation:
The old guardrail still holds. Residue should stay off in the early branch and in the late anchor-collapse branch.

#### 4. The best signal is localized inside the mid/late branch
Strongest localization pocket:
- stratifier: `boundary_depth_tercile`
- band: `mid`
- anchor-like gain mean: `+0.27001`

Other strong anchor-like pockets:
- `boundary_depth_tercile / low`: `+0.17301`
- `support_risk_tercile / low`: `+0.21701`
- `support_risk_tercile / mid`: `+0.20288`

Interpretation:
The mid/late branch is still too broad as a single note. The residue effect concentrates in a narrower middle-depth / lower-support-risk pocket.

#### 5. Residue is not just a late trailing symptom inside the mid/late branch
Anchor-like ordering result:
- dominant relation: `before_support_collapse`
- residue-vs-support centroid delta: `-0.05524`

Interpretation:
Inside the mid/late branch, residue tends to rise slightly before the main support-fragility centroid rather than after it. That supports calling it an auxiliary companion marker, not merely a trailing symptom, while still not making it a governing driver.

#### 6. Global non-promotion still holds
All slices:
- support-only failure Brier: `0.22274`
- branch-local auxiliary failure Brier: `0.22463`
- support-plus-residue failure Brier: `0.24537`

Anchor-like only:
- support-only failure Brier: `0.15390`
- branch-local auxiliary failure Brier: `0.15006`
- support-plus-residue failure Brier: `0.15535`

Interpretation:
There is a real local anchor-like policy gain, but once all families are recombined support-only remains the safest promoted global mechanism. Global residue blending is still clearly worse.

### Promote / Do Not Promote

Promote:
- residue has bounded auxiliary value inside the mid/late wedge support-collapse branch
- the effect is strongest in a narrower subregion, not across the whole branch
- early branch is robustly harmed by residue
- late anchor-collapse branch is harmed by residue in the anchor-like replay families
- support geometry remains the governing mechanism

Do not promote:
- residue as a whole-branch mid/late law
- residue as a global correction
- branch-local auxiliary policy as the new global default

### Best current wording
Wedge residue is not a second law and not a global correction. Its only reproducible positive role is as a bounded auxiliary marker inside a narrower subregion of the mid/late wedge support-collapse branch, while the globally promoted mechanism remains support geometry on the portable compact-validity axis.

### Recommended next step
`midlate_auxiliary_subregion_note`

Translation:
bank this as a carefully bounded local note, not as a new regime-wide or global policy claim.

## 2026-03-14 - RFTP-1.25 Branch Regime Map Refinement and Local Auxiliary Integration Test

### Ticket
`RFTP-1.25 - Branch Regime Map Refinement and Local Auxiliary Integration Test`

### Objective
Refine the 1.24 multi-branch compact-validity map conservatively and test whether residue can be used only as a branch-local auxiliary inside the mid/late wedge support-collapse branch without weakening the support-geometry mechanism picture.

### Fixed ingredients
- Canonical fixture: `repaired_anchor_canonical_v1`
- Frozen portable axis:
  - `slice_percentile_pair_max`
- Starting branch map from 1.24:
  - early wedge fragility `0.00-0.17`
  - mid/late wedge support-collapse `0.56-0.70`
  - late full-anchor support-collapse `0.70-0.90`
- Conservative sweep:
  - early upper `0.15 / 0.17 / 0.19`
  - mid/late lower `0.54 / 0.56 / 0.58`
  - mid/late upper `0.68 / 0.70 / 0.72`
  - late core upper `0.88 / 0.90 / 0.92`
- Operational policies compared:
  - global support-only
  - global support-plus-residue everywhere
  - branch-local auxiliary:
    - support-only in early
    - support-plus-residue only in mid/late
    - support-only in late

### Result
Classification: `midlate_local_auxiliary_supported_only`

Bottom line:
The branch-aware picture sharpens a little, but not enough to produce a stronger global operational policy. The only honest positive signal remains local:
- residue helps in the mid/late wedge support-collapse branch
- residue still hurts in the early branch
- residue is neutral-to-harmful in the late branch

So the paper-safe statement is:
residue remains globally non-governing, but it has a real auxiliary role inside the mid/late wedge branch only.

### Main Findings

#### 1. The best refined boundaries move only slightly
Best refinement:
- `e17_m58_x72_l88`

That means:
- early upper stays at `0.17`
- mid/late branch shifts outward to `0.58-0.72`
- late core cap relaxes slightly to `0.88`

Interpretation:
The 1.24 map was already close. The best refinement is a local cleanup, not a rediscovery.

#### 2. Refinement helps a little, but not enough to change the global story
Branch-local policy:
- best failure Brier: `0.19663`
- frozen 1.24 failure Brier: `0.19760`
- gain: `0.00097`

Calibration:
- best branch-local policy calibration MAE: `0.08987`
- frozen 1.24 calibration MAE: `0.09349`
- gain: `0.00362`

Interpretation:
There is some real refinement signal here, but the gain is too small to claim a materially stronger global regime policy.

#### 3. The refined branch-local policy does not beat global support-only overall
Transport means across the primary families:
- branch-local auxiliary failure Brier: `0.19663`
- global support-only failure Brier: `0.19618`
- branch-local minus support-only: `+0.00045` worse

Macro recall:
- branch-local auxiliary: `0.51307`
- global support-only: `0.52546`
- delta: `-0.01240`

Interpretation:
The best refined branch-local policy is not the new global winner. Support-only remains at least as good overall.

#### 4. Global support-plus-residue is still clearly worse
Transport means:
- global support-plus-residue failure Brier: `0.21274`
- branch-local auxiliary failure Brier: `0.19663`
- advantage of branch-local over global residue blend: `0.01611`

Interpretation:
Restricting residue locally matters. Turning it on globally still damages the operational object.

#### 5. Mid/late branch local utility is real
Mean AUROC gain in the mid/late branch:
- combined over support: `+0.03063`

Positive-family rate:
- `0.50`

Representative family-level behavior:
- `full_bootstrap`: support `0.5253` -> combined `0.7612`
- `full_subsample`: support `0.5705` -> combined `0.7200`
- `reference_full`: support `0.5843` -> combined `0.7512`

Interpretation:
There is a real local auxiliary effect in the mid/late branch, even though it does not upgrade the full transported policy.

#### 6. Early and late branches still reject residue
Early branch:
- combined gain vs support mean: `-0.25964`

Late branch:
- combined gain vs support mean: `-0.01861`

Interpretation:
This remains a strict locality result. Residue should stay off outside the mid/late wedge branch.

#### 7. Gap structure still matters
Gap-region failed rates under the best refined map:
- early-to-mid gap: `0.2194`
- mid/late-to-late transition: `0.4180`

Wedge fraction in those regions:
- early-to-mid gap: `0.1304`
- mid/late-to-late transition: `0.2746`

Interpretation:
The remaining partial-transport problem still looks like transition smearing, not a failure of the support geometry story.

### Promote / Do Not Promote

Promote:
- the branch-aware regime picture is stable enough to use
- residue has branch-confined auxiliary utility in the mid/late wedge branch
- support geometry remains the governing mechanism
- residue should not be treated as a global law or global correction

Do not promote:
- the refined branch-local policy as the new global operational default
- any claim that residue improves compact validity outside the mid/late branch
- any claim that the small boundary shifts materially change the scientific picture

### Best current wording
The portable support-risk axis remains the governing compact-validity ordering object. A lightly refined multi-branch regime map sharpens that picture, and wedge residue shows real but strictly local auxiliary utility inside the mid/late wedge support-collapse branch only. It does not improve the global transported support-only policy and should not be promoted as a global mechanism.

### Recommended next step
`midlate_branch_auxiliary_note`

Translation:
bank the local mid/late auxiliary result cleanly, but do not escalate it into a global law or policy claim.

## 2026-03-14 - RFTP-1.24 Multi-Branch Regime Map and Branch-Conditioned Utility Test

### Ticket
`RFTP-1.24 - Multi-Branch Regime Map and Branch-Conditioned Utility Test`

### Objective
Turn the 1.23 branch discovery into the first branch-aware compact-validity map on the frozen portable risk axis, compare it directly against the older safe/stressed/high-risk threshold gate, and test whether residue has only conditional local utility rather than global governing status.

### Fixed ingredients
- Canonical fixture: `repaired_anchor_canonical_v1`
- Frozen portable axis:
  - `slice_percentile_pair_max`
- Frozen branch cores from 1.23:
  - early wedge fragility `0.00-0.17`
  - mid/late wedge support-collapse `0.56-0.70`
  - late full-anchor support-collapse core `0.70-0.90`
- Operational regime map:
  - early branch
  - stable interior gap `0.17-0.56`
  - mid/late wedge branch
  - late branch plus tail `>= 0.70`
- Comparison baseline:
  - 1.21 threshold gate using the frozen source-fit thresholds

### Result
Classification: `branch_map_transport_partial`

Bottom line:
The frozen branch map is stable enough to use and it does beat the old threshold gate, but only modestly. The strong safe claim is:
- branch-aware interpretation is better than the single threshold gate
- but the operational gain is not yet large enough to call the branch map finished

### Main Findings

#### 1. The branch map is stable under light boundary perturbation
Mean robustness delta across the small shift / widen / narrow tests:
- `0.0216`

Interpretation:
The three-branch picture is not fragile to tiny band changes. That is good enough for a paper-safe regime interpretation.

#### 2. The branch map improves transport over the old threshold gate
Average transport metrics:
- threshold gate failure Brier mean: `0.2361`
- branch map failure Brier mean: `0.2337`
- Brier gain: `0.00239`

Calibration:
- threshold gate group calibration MAE mean: `0.1494`
- branch map group calibration MAE mean: `0.1413`
- calibration gain: `0.00813`

Interpretation:
The branch-aware object is better than the old thresholded gate, but the margin is still incremental rather than decisive.

#### 3. The regime map is readable and operational
The branch-aware map now has four usable regimes:
- early wedge fragility
- stable interior / non-branch gap
- mid/late wedge support-collapse
- late full-anchor support-collapse plus tail

Representative occupancy on the source slice:
- early branch: `239` states
- stable interior gap: `735`
- mid/late wedge branch: `240`
- late branch plus tail: `671`

Interpretation:
This is now a genuine regime map, not just a single trust curve with a blurry shoulder.

#### 4. Residue stays non-governing globally, but it is locally useful in the mid/late wedge branch
Mid/late branch utility:
- support only AUROC mean: `0.5557`
- residue only: `0.5954`
- support + residue: `0.6110`

By contrast:
- early branch:
  - support `0.6924`
  - support + residue `0.4327`
- late branch:
  - support `0.5636`
  - support + residue `0.5446`

Interpretation:
This is the cleanest version of the residue story so far:
- residue is still not a global mechanism
- but it does become locally helpful inside the mid/late wedge support-collapse branch
- that local gain does not generalize to the early or late branches

#### 5. Transition geometry is mixed, not cliff-like
Mean transition jumps:
- early-to-interior failure jump: `0.0623`
- midlate-to-late failure jump: `-0.0217`

And in wedge-matched slices:
- interior-to-midlate jumps are large and positive
- midlate-to-late jumps can flatten or reverse

Interpretation:
The regime map is real, but it is not organized by one universal cliff. The early branch is the most discrete transition; the later support-collapse structure is more graded and family-dependent.

### Paper-facing interpretation
This is a useful upgrade, even though it is not the final regime object.

The cleanest current statement is:
- the portable axis remains the global ordering object
- the branch map is the right regime structure on top of that axis
- support geometry is still the main governing mechanism
- residue is only a local auxiliary signal in the mid/late wedge support-collapse branch

### Promotion guidance
Promote:
- the frozen three-branch structure as the current best regime interpretation
- the fact that branch-aware mapping modestly outperforms the earlier threshold gate
- residue as local auxiliary utility only in the mid/late wedge branch
- the conclusion that later breakdown is still more graded than cliff-like

Do not promote:
- the branch map as the final operational gate
- residue as a global governing law
- a claim that all branch transitions are sharp or universal

### Best next step
`branch_regime_map_refinement`

What 1.25 should probably do:
- refine the branch transport/calibration object rather than searching new laws
- decide whether the late branch should stay one band-plus-tail or split into a cleaner transported late-core vs tail object
- keep residue confined to the mid/late wedge branch unless new evidence appears

### Artifacts
- Summary:
  - `results/20260314_202015_wedge_multi_branch_regime_map_v1_s20000_seed26/wedge_multi_branch_summary.json`
- Regime map:
  - `results/20260314_202015_wedge_multi_branch_regime_map_v1_s20000_seed26/wedge_multi_branch_regime_map.csv`
- Transition structure:
  - `results/20260314_202015_wedge_multi_branch_regime_map_v1_s20000_seed26/wedge_branch_transition_structure.csv`
- Branch-conditioned utility:
  - `results/20260314_202015_wedge_multi_branch_regime_map_v1_s20000_seed26/wedge_branch_conditioned_utility.csv`
- Transport calibration:
  - `results/20260314_202015_wedge_multi_branch_regime_map_v1_s20000_seed26/wedge_branch_transport_calibration.csv`
- Boundary robustness:
  - `results/20260314_202015_wedge_multi_branch_regime_map_v1_s20000_seed26/wedge_branch_boundary_robustness.csv`

## 2026-03-14 - RFTP-1.23 Failure-Branch Stratification on the Portable Risk Axis

### Ticket
`RFTP-1.23 - Failure-Branch Stratification on the Portable Risk Axis`

### Objective
Resolve the `multiple_failure_regimes` result from 1.22 into explicit structural breakdown branches on the frozen portable support-risk axis, without replacing the axis or reopening wedge-law search.

### Fixed ingredients
- Canonical fixture: `repaired_anchor_canonical_v1`
- Frozen portable axis:
  - `slice_percentile_pair_max`
- Same slice family as 1.20-1.22:
  - reference full slice
  - full-anchor bootstrap and subsample transport
  - wedge-matched transport slices
  - wedge-only and nonwedge matched controls
- Branch bands extracted from the observed 1.22 slope peaks

### Result
Classification: `multi_branch_structure_supported`

Bottom line:
The portable risk axis does not reduce to a single late support-collapse edge or a simple two-branch split. It supports at least three reproducible structural bands:
- early wedge fragility: `0.00-0.17`
- mid/late wedge support-collapse: `0.56-0.70`
- late full-anchor support-collapse: `0.70-0.90`

### Main Findings

#### 1. The candidate branch bands are reproducible
Recovered branch bands:
- `early_wedge_fragility_branch`: center `0.10`, band `0.00-0.17`
- `midlate_wedge_support_branch`: center `0.63`, band `0.56-0.70`
- `late_full_anchor_support_branch`: center `0.832`, band `0.70-0.90`

Interpretation:
These bands line up directly with the recurrent 1.22 slope structure instead of coming from a new coordinate or clustering pass.

#### 2. Early fragility is structurally distinct from both later branches
Best early-vs-late discriminators:
- `intersection_rank_mean`: AUROC `0.9990`
- `boundary_depth`: AUROC `0.9957`

Best early-vs-midlate discriminators:
- `intersection_rank_mean`: AUROC `1.0000`
- `boundary_depth`: AUROC `1.0000`

Interpretation:
The early branch is not just a smeared tail of the late support-collapse regime. Support geometry separates it almost perfectly.

#### 3. Mid/late wedge collapse is not the same as the late full-anchor branch
Best midlate-vs-late discriminator:
- `intersection_rank_mean`: AUROC `0.7938`

Also:
- `boundary_depth`: AUROC `0.7446`

Interpretation:
The wedge-matched later branch and the late full-anchor branch are related, but not identical. That is why 1.23 stays at multi-branch rather than promoting a clean two-branch collapse.

#### 4. Branch signatures track different failure severities
Average failed rates by family:
- early branch:
  - wedge-matched `0.1879`
  - full-anchor families about `0.0000-0.0052`
- mid/late wedge branch:
  - wedge-matched `0.5587`
  - full-anchor families about `0.2048-0.2091`
- late full-anchor branch:
  - reference/full families about `0.3686-0.4229`
  - wedge-matched `0.6499`

Interpretation:
The early band behaves like a wedge-local fragility pocket, while the two later bands are genuine support-collapse regimes with different severity and geometry.

#### 5. Branch identity is still support-geometric
Across pairwise branch separation, the leading discriminators stayed support variables:
- `intersection_rank_mean`
- `boundary_depth`

Interpretation:
The branch structure is still being organized by support geometry, not by a promoted wedge law.

#### 6. Residue remains non-defining, but becomes locally more competitive in the mid/late branch
Branch-level AUROC means:
- early branch:
  - support only `0.7158`
  - residue only `0.3924`
  - support + residue `0.4737`
- late full-anchor branch:
  - support only `0.5379`
  - residue only `0.4829`
  - support + residue `0.4998`
- mid/late wedge branch:
  - support only `0.5556`
  - residue only `0.5802`
  - support + residue `0.5954`

Interpretation:
Residue still does not define the branches, but after mixture separation it is no longer uniformly irrelevant. The mid/late wedge support-collapse branch is the one place where residue starts to carry local lift.

### Paper-facing interpretation
This ticket upgrades the current picture from:
- one portable trust coordinate with a broad frontier

to:
- one portable trust coordinate with multiple structural failure branches

The cleanest current statement is:
- compact breakdown is organized by a portable support-risk axis
- that axis contains at least an early wedge-local fragility branch and two later support-collapse bands
- branch identity is still mainly support-geometric
- wedge residue is not the governing law, but it becomes locally more informative once the support-collapse mixture is separated

### Promotion guidance
Promote:
- the existence of multiple structural breakdown branches on the portable risk axis
- the early wedge fragility branch as a distinct support-geometric regime
- the fact that `intersection_rank_mean` and `boundary_depth` separate branch identity strongly
- the conclusion that a single-threshold frontier is too simple for the branch structure now visible

Promote with caution:
- residue as a local branch diagnostic inside the mid/late wedge support-collapse branch only

Do not promote:
- a clean two-branch collapse of the whole system
- wedge residue as a branch-defining mechanism
- a final universal branch threshold map

### Best next step
`multi_branch_regime_map`

What 1.24 should probably do:
- formalize the branch-aware compact validity map
- distinguish the early fragility pocket from the two later collapse bands
- decide whether the mid/late wedge branch and late full-anchor branch should be treated as separate operational regimes or one family with shifted severity

### Artifacts
- Summary:
  - `results/20260314_193915_wedge_failure_branch_stratification_v1_s20000_seed26/wedge_failure_branch_summary.json`
- Branch profiles:
  - `results/20260314_193915_wedge_failure_branch_stratification_v1_s20000_seed26/wedge_failure_branch_profiles.csv`
- Branch discrimination:
  - `results/20260314_193915_wedge_failure_branch_stratification_v1_s20000_seed26/wedge_branch_discrimination.csv`
- Branch consistency:
  - `results/20260314_193915_wedge_failure_branch_stratification_v1_s20000_seed26/wedge_branch_consistency.csv`
- Branch ablation:
  - `results/20260314_193915_wedge_failure_branch_stratification_v1_s20000_seed26/wedge_branch_ablation.csv`

## 2026-03-14 - RFTP-1.22 Compact Breakdown Frontier Mapping

### Ticket
`RFTP-1.22 - Compact Breakdown Frontier Mapping`

### Objective
Map the geometry of compact-law breakdown along the frozen portable support-risk axis from 1.20 / 1.21, without forcing final thresholds, and determine whether the boundary looks sharp, band-like, or multi-regime.

### Fixed ingredients
- Canonical fixture: `repaired_anchor_canonical_v1`
- Frozen portable axis:
  - `slice_percentile_pair_max`
- Support features:
  - `intersection_rank_mean`
  - `boundary_depth`
- Same slice family as 1.20 / 1.21:
  - reference full slice
  - full-anchor bootstrap and subsample transport
  - wedge-matched transport slices
  - wedge-only and nonwedge controls
- Frontier estimator:
  - Gaussian kernel smoothing
  - bandwidth: `0.06`
  - grid size: `51`

### Result
Classification: `multiple_failure_regimes`

Bottom line:
There is not one universal compact-breakdown edge on the portable risk axis. Full-anchor slices align on a late broad frontier near high risk, while wedge-matched slices consistently split into an earlier and later breakdown structure.

### Main Findings

#### 1. Full-anchor frontier geometry is stable
Across the reference plus full-anchor resamples:
- peak slope location: about `0.82-0.84`
- full-anchor peak-location std: `0.0098`
- transition width: about `0.45-0.49`

Interpretation:
The full repaired-anchor transport family has a very stable late breakdown band. That part of the frontier is real and portable.

#### 2. Wedge-matched slices split into two regimes
For both wedge-matched slices:
- peak slope location: `0.10`
- second significant peak: about `0.62-0.64`
- significant peak count: `2` on both slices
- `wedge_matched_multi_regime_rate = 1.0`

Interpretation:
The wedge-matched transport family does not collapse onto the same single boundary as the full-anchor family. It shows a reproducible early-plus-late breakdown structure instead.

#### 3. The frontier is broad, not threshold-sharp
Across primary slices:
- transition width mean: `0.4936`
- transition width std: `0.0419`
- peak slope mean: `2.0050`

Interpretation:
Even where the frontier is stable, it behaves more like a broad transition band than a razor-sharp threshold. That reinforces the 1.21 result that the ordering is portable before the thresholds are final.

#### 4. Wedge overlap is real, but not the whole story
Using the steep-slope shoulder rather than the whole 20-80 band:
- frontier wedge enrichment mean: `1.2371`

Interpretation:
Wedge states do cluster on the breakdown frontier shoulder, but they do not define the entire frontier by themselves. That keeps the interpretation aligned with the support-risk mechanism rather than a wedge-only chart.

#### 5. Residue is still not the governing frontier variable
Residue behavior did not settle into a clean universal "after-frontier" lag:
- `residue_after_frontier_rate = 0.0` across the primary aggregate

More specifically:
- full-anchor slices show residue peaking well before the late broad frontier
- wedge-matched slices place the residue peak inside the later regime, not at the early one

Interpretation:
Residue remains useful as a local diagnostic, but 1.22 does not support promoting it as the portable frontier-defining quantity.

### Paper-facing interpretation
This ticket sharpens the story substantially:
- the portable support-risk coordinate is real
- the breakdown frontier is real
- but it is not a single universal threshold edge

The cleanest current statement is:
- full-anchor compact breakdown follows a stable late probabilistic frontier band
- wedge-matched transport reveals an additional earlier breakdown regime
- therefore the compact breakdown geometry is multi-regime, not single-threshold

### Promotion guidance
Promote:
- the existence of a stable late full-anchor breakdown frontier
- the wedge-matched evidence for a second breakdown regime
- the conclusion that the compact breakdown frontier is multi-regime
- the support-risk-axis framing as the right coordinate for breakdown geometry

Do not promote:
- a single final threshold boundary
- wedge residue as the portable frontier law
- a claim that wedge alone defines the breakdown frontier

### Artifacts
- Summary:
  - `results/20260314_191906_wedge_frontier_mapping_v1_s20000_seed26/wedge_frontier_summary.json`
- Frontier curve:
  - `results/20260314_191906_wedge_frontier_mapping_v1_s20000_seed26/wedge_breakdown_frontier_curve.csv`
- Frontier density:
  - `results/20260314_191906_wedge_frontier_mapping_v1_s20000_seed26/wedge_frontier_density.csv`
- Frontier alignment:
  - `results/20260314_191906_wedge_frontier_mapping_v1_s20000_seed26/wedge_frontier_alignment.csv`
- Residue behavior:
  - `results/20260314_191906_wedge_frontier_mapping_v1_s20000_seed26/wedge_residue_frontier_behavior.csv`
- Width estimate:
  - `results/20260314_191906_wedge_frontier_mapping_v1_s20000_seed26/wedge_frontier_width_estimate.csv`

### One-sentence research memory
`RFTP-1.22` says the portable support-risk axis hosts a real compact-breakdown frontier, but that frontier is multi-regime: a stable late broad band on full-anchor transport plus an additional earlier breakdown regime in wedge-matched slices.

## 2026-03-14 - RFTP-1.21 Portable Risk-Gated Compact Validity Test

### Ticket
`RFTP-1.21 - Portable Risk-Gated Compact Validity Test`

### Objective
Test whether the frozen 1.20 portable support-risk axis can be used as an operational compact-validity gate that separates compact-safe, compact-stressed, and compact-high-risk states across the canonical transport family.

### Fixed ingredients
- Canonical fixture: `repaired_anchor_canonical_v1`
- Frozen portable axis:
  - `slice_percentile_pair_max`
- Frozen support features:
  - `intersection_rank_mean`
  - `boundary_depth`
- Frozen source thresholds from the reference slice:
  - stress quantile: `0.50`
  - fail quantile: `0.60`
  - stress threshold: `0.5366`
  - fail threshold: `0.6545`

### Result
Classification: `partial_gate_transport`

Bottom line:
The portable axis is good enough to act as a meaningful compact-validity gradient, but not yet strong enough to claim as a fully portable sharp threshold gate. In paper terms, it currently promotes as a trust coordinate more cleanly than as a universal regime map.

### Main Findings

#### 1. The compact-validity gradient is real
Across transport slices:
- transport macro recall mean: `0.5024`
- mixed-slice macro recall mean: `0.5333`
- trust failed-rate monotonicity mean: `0.7300`
- trust severity monotonicity mean: `0.8424`

Interpretation:
Compact-law quality does stratify in the right direction as portable risk rises. The signal is real enough to be useful operationally, especially as an ordering coordinate.

#### 2. The source trust curve is very clean
On the reference slice:
- decile 1 failed rate: `0.0000`
- decile 10 failed rate: `0.6032`
- decile 1 wedge fraction: `0.0000`
- decile 10 wedge fraction: `0.9312`

Interpretation:
Within the source slice, the risk axis behaves exactly like a compact-trust coordinate should: low risk looks interior and safe, while the highest-risk tail concentrates both wedge states and compact failure.

#### 3. Wedge states are concentrated in the high-risk tail on mixed transport
On wedge-matched transport:
- mixed high-risk wedge enrichment mean: `1.5334`
- mixed wedge high-risk capture rate mean: `0.6866`
- mixed failed overcall mean: `-0.0390`

Interpretation:
The high-risk bin is genuinely wedge-enriched and captures most wedge states, but wedge is not identical to the high-risk tail. That is exactly the stronger interpretation we wanted.

#### 4. The thresholds are usable, but not yet clean enough to call fully portable
On mixed transport:
- macro recall mean: `0.5333`
- failed-rate overcall mean: `-0.0390`

What held back promotion:
- the transported ordering is good, but the cross-slice failed-rate monotonicity average only reached `0.7300`, below the stronger “portable gate confirmed” bar
- the frozen thresholds are serviceable, but not yet robust enough to present as a final universal regime map

Interpretation:
This is a partial win. The axis transports better as a ranked trust coordinate than as a final frozen threshold rule.

#### 5. Residue stayed irrelevant under gating
Across whole-slice checks:
- `support_beats_residue_rate = 1.0`
- `combined_nonpositive_rate = 1.0`

Interpretation:
Even after the correct portable risk coordinate is introduced, wedge residue still adds zero or negative lift. That further reinforces the paper-safe picture that residue is a symptom marker, not part of the governing compact-validity mechanism.

### Paper-facing interpretation
This ticket strengthens the 1.20 result, but in a specific way:
- promote the portable support-risk axis as a compact-validity ordering coordinate
- do not yet promote the frozen thresholds as a final transported safe/stressed/failed regime law

The safest current language is:
- compact validity degrades monotonically with a portable normalized support-risk coordinate
- wedge states concentrate in the high-risk tail of that coordinate
- wedge residue remains symptom-like and adds no lift
- the exact operational threshold map still needs refinement

### Promotion guidance
Promote:
- the portable risk axis as a trust / ordering coordinate
- the clean source trust-curve separation
- the wedge-high-risk enrichment result
- the repeated residue-nonadditivity result

Do not promote:
- the exact frozen threshold set as a final portable operational gate
- any claim that the safe/stressed/high-risk boundaries are fully settled across slices

### Artifacts
- Summary:
  - `results/20260314_191019_wedge_risk_gate_v1_s20000_seed26/wedge_risk_gate_summary.json`
- Compact-validity bins:
  - `results/20260314_191019_wedge_risk_gate_v1_s20000_seed26/wedge_risk_gated_compact_validity.csv`
- Threshold transport:
  - `results/20260314_191019_wedge_risk_gate_v1_s20000_seed26/wedge_risk_threshold_transport.csv`
- Trust curve:
  - `results/20260314_191019_wedge_risk_gate_v1_s20000_seed26/wedge_compact_trust_curve.csv`
- Residue re-check:
  - `results/20260314_191019_wedge_risk_gate_v1_s20000_seed26/wedge_risk_residue_check.csv`
- Bin calibration:
  - `results/20260314_191019_wedge_risk_gate_v1_s20000_seed26/wedge_risk_bin_calibration.csv`

### One-sentence research memory
`RFTP-1.21` says the portable support-risk axis is already a real compact-validity trust coordinate, but its frozen thresholds are not yet strong enough to promote as the final transported regime gate.

## 2026-03-14 - RFTP Sync Note: Global Physics Targets from Pioneer

### Status
Stored as orientation anchors only. Not used as fitting targets for the active wedge / compact-validity lane.

### Canonical file
- `polytope_global_targets.json`

### Synced targets
- Gauge-sector simplex weights:
  - `U1 = 0.25`
  - `SU2 = 0.30`
  - `SU3 = 0.45`
- Weak-sector geometric anchor:
  - `sin^2(theta_W) = 5/23 ~= 0.217391`
- Geometry energy scale:
  - `~1e10 GeV`

### Operational rule
- These values are global orientation anchors for future polytope / facet-normalization work.
- They are not constraints for the current Codex wedge, compact-validity, or portable-risk-axis tickets.
- If geometric weak-angle values differ from the lab-scale `sin^2(theta_W)(M_Z) ~= 0.2312`, treat renormalization-group running as the first explanation, not local support collapse.

### Paper-facing interpretation
The lanes are now cleanly separated:
- Pioneer track:
  - discovers candidate global facet targets
- Codex refinement track:
  - maps stability, validity, and breakdown geometry inside the polytope

This is a good synchronization boundary because discovery is informing orientation without directly tuning the refinement search.

## 2026-03-14 - RFTP-1.20 Surface Renormalization and Portable Risk Coordinate Test

### Ticket
`RFTP-1.20 - Surface Renormalization and Portable Risk Coordinate Test`

### Objective
Test whether the transport failure from 1.19 was mainly a coordinate/calibration problem rather than a mechanism failure, by replacing the raw transported surface with normalized support-risk coordinates built from the 1.18/1.19 support variables.

### Fixed ingredients
- Canonical fixture: `repaired_anchor_canonical_v1`
- Frozen mechanism from 1.18 / 1.19:
  - primary support feature: `intersection_rank_mean`
  - companion support feature: `boundary_depth`
- Raw transported surface used as the comparison baseline:
  - source support feature: `intersection_rank_mean`
  - source wedge feature: `wedge_residue_score`
- Same transport family as 1.19:
  - full-anchor resamples
  - wedge-matched slices
  - wedge-only transport checks
  - matched nonwedge controls

### Result
Classification: `portable_risk_coordinate_identified`

Bottom line:
The mechanism did survive renormalization. A normalized support-risk coordinate transported materially better than the raw 1.18 surface on wedge-matched slices, while keeping the support-vs-residue interpretation intact.

### Main Findings

#### 1. The best portable coordinate is support-only and simple
Best coordinate:
- `slice_percentile_pair_max`

Definition:
- take within-slice percentile-normalized `intersection_rank_mean`
- take within-slice percentile-normalized `boundary_depth`
- use the `max` of the two as the scalar risk axis

Interpretation:
The portable object is not the old raw 2D transported plane. It is a monotone, slice-normalized support-risk coordinate built entirely from support-collapse geometry.

#### 2. Wedge-matched transport improved substantially
For the best coordinate on `mixed_transport`:
- no-retune macro recall: `0.4956`
- raw 1.19 surface macro recall: `0.3419`
- macro recall gain vs raw: `+0.1537`

Overcall:
- best coordinate no-retune overcall: `-0.0613`
- raw surface no-retune overcall: `+0.2145`
- overcall reduction vs raw: `0.2758`

Interpretation:
This is the key positive result. The wedge-matched transport failure was mostly a bad coordinate problem, not a broken mechanism.

#### 3. Light recalibration was not needed for the winner
Best coordinate on mixed transport:
- no-retune macro recall: `0.4956`
- light recalibration macro recall: `0.4751`
- light recalibration gain: `-0.0205`

Interpretation:
The best coordinate is already sufficiently normalized that light threshold recalibration actually hurts. That is strong evidence that portability improved at the coordinate level, not just by threshold repair.

#### 4. The shift decomposition explains why the raw surface failed
On wedge-matched slices, the raw transported surface saw:
- support location shift: about `+0.42`
- support scale ratio: about `0.70-0.73`
- companion location shift: about `+0.47-0.48`
- companion scale ratio: about `0.70-0.74`
- failed-rate delta: about `+0.25`
- wedge-fraction delta: `+0.3095`

Interpretation:
The no-retune failure in 1.19 was mostly caused by strong location shift plus scale compression in the support predictors, not by a collapse of the support mechanism itself.

#### 5. The symptom-vs-cause split survived again
For the best mixed-transport coordinate:
- `support_beats_residue_rate = 1.0`
- `combined_nonpositive_rate = 1.0`

Interpretation:
Even after renormalization, wedge residue still adds zero or negative lift once support geometry is in the right coordinate system. That strengthens the paper claim that wedge residue is a symptom marker, not the portable mechanism.

#### 6. The renormalized winner slightly changes local dominance
On mixed transport for the best coordinate:
- `intersection_feature_auroc_mean = 0.6319`
- `boundary_depth` companion AUROC mean = `0.6367`
- `intersection_dominance_rate = 0.0`

Interpretation:
After normalization, `intersection_rank_mean` is no longer the sole local transport leader inside wedge-matched slices. The portable coordinate works because the mechanism is genuinely two-feature support-collapse geometry, not because one raw feature stays dominant everywhere.

### Paper-facing interpretation
This ticket upgrades the support-collapse story from:
- mechanism yes, surface maybe

to:
- mechanism yes, portable coordinate identified

The safest paper language now is:
- the wedge sector is best understood as a localized compact-law breakdown regime
- the portable predictor is a normalized support-risk coordinate
- wedge residue remains a symptom marker and not part of the portable mechanism

### Promotion guidance
Promote:
- the renormalized support-risk coordinate result
- the specific winner `slice_percentile_pair_max`
- the shift-decomposition explanation that raw transport failed because of location and scale drift
- the repeated negative ablation that wedge residue still adds zero or negative lift after renormalization

Do not promote:
- the original raw 1.18 2D surface as the portable object
- any claim that wedge residue belongs in the portable transported rule

### Artifacts
- Summary:
  - `results/20260314_184802_wedge_surface_renormalization_v1_s20000_seed26/wedge_surface_renormalization_summary.json`
- Shift decomposition:
  - `results/20260314_184802_wedge_surface_renormalization_v1_s20000_seed26/wedge_transport_shift_decomposition.csv`
- Coordinate sweep:
  - `results/20260314_184802_wedge_surface_renormalization_v1_s20000_seed26/wedge_normalized_coordinate_sweep.csv`
- Portable risk-axis leaderboard:
  - `results/20260314_184802_wedge_surface_renormalization_v1_s20000_seed26/wedge_portable_risk_axis.csv`
- Renormalized ablation:
  - `results/20260314_184802_wedge_surface_renormalization_v1_s20000_seed26/wedge_normalized_ablation.csv`

### One-sentence research memory
`RFTP-1.20` says the support-collapse mechanism really is portable after renormalization, and the right transported object is a slice-normalized support-risk axis (`slice_percentile_pair_max`), not the original raw surface and not a support-plus-residue blend.

## 2026-03-14 - RFTP-1.19 Breakdown Surface Replication and Transport Test

### Ticket
`RFTP-1.19 - Breakdown Surface Replication and Transport Test`

### Objective
Test whether the 1.18 compact-breakdown surface is portable beyond the exact source slice by carrying the frozen support rule, thresholds, and support-vs-residue comparison across nearby canonical-anchor resamples and matched wedge/nonwedge transport slices.

### Fixed ingredients
- Canonical fixture: `repaired_anchor_canonical_v1`
- Source support predictor: `intersection_rank_mean`
- Source wedge diagnostic: `residue_ranked_log_pole_asymmetry__linear__k12`
- Frozen 1.18 surface:
  - support threshold quantile: `0.65`
  - wedge threshold quantile: `0.35`
- Label policy:
  - compact failure defined by frozen compact-rank-error thresholds from 1.18

### Result
Classification: `replication_mixed`

Bottom line:
The support-breakdown story survives cleanly on full-anchor resamples, but transport gets materially weaker on matched wedge/nonwedge slices. So the mechanism looks real, but not yet portable enough to promote as a fixture-agnostic structural surface.

### Main Findings

#### 1. The support-vs-residue result replicated perfectly
Across all transported slices:
- `support_beats_residue_rate = 1.0`
- `combined_nonpositive_rate = 1.0`

Interpretation:
The strongest stable part of 1.18 replicated completely. Support geometry kept beating wedge residue everywhere, and adding wedge residue never improved prediction once support geometry was present.

#### 2. `intersection_rank_mean` stayed near the top, but not always at the top
Across transported slices:
- top-1 rate: `0.50`
- top-2 rate: `0.80`

What changed:
- full resamples kept `intersection_rank_mean` at rank `1`
- wedge-matched transport slices demoted it to rank `2`
- wedge-only slices were symptom-dominated and put `wedge_residue_score` at rank `2`, with `rank_asymmetry` taking rank `1`

Interpretation:
The support mechanism remains central, but the exact single-feature dominance weakens once the slice is forced into wedge-heavy local transport.

#### 3. Full-anchor replication was strong
On the full-anchor bootstrap and subsample slices:
- `intersection_rank_mean` stayed rank `1`
- support-only AUROC stayed around `0.807-0.815`
- wedge-residue-only AUROC stayed around `0.590-0.619`
- surface-shape preservation was strong:
  - failed-rate Spearman vs source: `0.947-0.995`
  - dominant-label agreement vs source: `0.8-1.0`

Interpretation:
The 1.18 mechanism is not a single-run accident. It is stable under nearby full-anchor resampling.

#### 4. Transport weakened on wedge-matched slices
For `wedge_plus_matched_nonwedge` transport slices:
- wedge failure enrichment fell to about `1.13-1.20`
- `intersection_rank_mean` dropped to rank `2`
- support-only AUROC dropped to about `0.623-0.641`
- no-retune rule macro recall dropped to about `0.340-0.343`
- predicted-failed fraction inflated to about `0.716-0.728`

Interpretation:
This is the main portability failure. The frozen source rule overcalls failure once the slice is forced into wedge-heavy matched transport, so the source surface is not yet cleanly transportable as-is.

#### 5. Threshold transport was only modestly recoverable
Across transported slices:
- no-retune macro recall mean: `0.3960`
- light recalibration macro recall mean: `0.4134`
- recalibration gain: `+0.0174`

Interpretation:
There is some threshold sensitivity, but only modest improvement from light recalibration. The main issue is not just a simple threshold offset.

### Paper-facing interpretation
This ticket strengthens the mechanism claim but weakens the portability claim.

What is now safe to say:
- the wedge regime still looks like a localized compact-law breakdown regime driven mainly by support collapse
- support geometry consistently outpredicts wedge residue
- wedge residue remains symptom-like because it adds no useful lift once support geometry is known

What is not yet safe to say:
- that the full 1.18 breakdown surface transports cleanly as a general low-dimensional rule without local caveats

### Promotion guidance
Promote:
- the replication of the support-vs-residue asymmetry
- the full-anchor resampling stability result
- the negative result that wedge residue still adds zero or negative lift after support geometry is known

Do not promote yet:
- the claim that the exact 1.18 2D breakdown surface is portable as a general predictor manifold
- the source thresholds as reusable cross-slice defaults

### Artifacts
- Summary:
  - `results/20260314_183827_wedge_breakdown_replication_v1_s20000_seed26/wedge_breakdown_replication_summary.json`
- Replication rows:
  - `results/20260314_183827_wedge_breakdown_replication_v1_s20000_seed26/wedge_breakdown_replication.csv`
- Threshold transport:
  - `results/20260314_183827_wedge_breakdown_replication_v1_s20000_seed26/wedge_threshold_transport.csv`
- Predictor rank stability:
  - `results/20260314_183827_wedge_breakdown_replication_v1_s20000_seed26/wedge_predictor_rank_stability.csv`
- Surface transport:
  - `results/20260314_183827_wedge_breakdown_replication_v1_s20000_seed26/wedge_surface_transport.csv`

### One-sentence research memory
`RFTP-1.19` says the support-breakdown mechanism is real and replicates on full-anchor resamples, but the exact wedge breakdown surface is only partially transportable, so promote the mechanism and the symptom-vs-cause separation, not the surface as a universal rule.

## 2026-03-14 - RFTP-1.18 Wedge Failure Predictor and Compact-Law Breakdown Surface

### Ticket
`RFTP-1.18 - Wedge Failure Predictor and Compact-Law Breakdown Surface`

### Objective
Test whether the wedge exception is better understood as a compact-law breakdown regime than as a second law or a boundary chart, by finding the smallest structural predictor set that flags compact breakdown inside and around the wedge zone.

### Fixed ingredients
- Canonical fixture: `repaired_anchor_canonical_v1`
- Primary region: `shared_overlap_or_contrast_pair`
- Wedge focus: `wedge_sharpness_high`
- Reference compact law: `shared_intersection_rank_concentration`
- Wedge residue used only as a diagnostic marker:
  - `residue_ranked_log_pole_asymmetry__linear__k12`

### Result
Classification: `support_breakdown_surface_identified`

Bottom line:
This lane supports the breakdown-regime interpretation. A small structural support panel predicts compact breakdown well, wedge failure is strongly enriched inside that regime, and the wedge residue adds no useful lift once support geometry is known.

### Label Definition
The important change in this ticket was the breakdown label itself.

State labels were not based on raw compact score. That first attempt missed the wedge zone.

The final label used:
- compact rank error against residual ground-truth ordering

Operationally:
- compute compact-law rank within each target on the repaired anchor
- compute residual-ppm rank within the same target
- define compact rank error = compact rank minus residual rank
- more negative means the compact law is overpromoting that state relative to the residual ordering

Ordinal label:
- `compact_failed`: bottom `25%` of rank-error values
- `compact_stressed`: up to the `60%` quantile
- `compact_stable`: remainder

This was the first labeling scheme that actually exposed the wedge regime instead of washing it out.

### Main Findings

#### 1. Wedge failure is strongly enriched in the compact-breakdown class
- wedge failed rate: `0.5460`
- non-wedge failed rate: `0.1809`
- wedge failure enrichment: `3.02x`

Interpretation:
Once compact failure is defined as overpromotion relative to residual ranking, the wedge region stands out clearly as a localized breakdown regime.

#### 2. One structural feature is already a strong early-warning predictor
Best support feature:
- `intersection_rank_mean`

Metrics:
- failed AUROC: `0.8096`
- severity Spearman: `0.5053`
- top-decile failure rate: `0.6085`
- top-decile failure enrichment: `2.43x`
- top-decile wedge fraction: `0.8624`

Interpretation:
This is the strongest result of the ticket. A single structural quantity already predicts compact breakdown substantially better than the wedge residue signal.

#### 3. Support variables outperform wedge residue variables cleanly
Support-only panel:
- failed AUROC: `0.8096`

Wedge-residue-only panel:
- failed AUROC: `0.6168`

Combined support + wedge residue:
- failed AUROC: `0.7566`
- delta vs support-only: `-0.0530`

Interpretation:
The wedge residue does not add unique predictive power here. It actually hurts the simple support-only panel. That strongly supports the interpretation that wedge residue is mostly a symptom marker of breakdown, not the primary cause variable.

#### 4. The best readable surface is real but still coarse
Best simple two-axis rule:
- support feature: `intersection_rank_mean`
- second axis: wedge residue risk

Metrics:
- accuracy: `0.4599`
- macro recall: `0.4781`
- failed F1: `0.5622`
- predicted-failed wedge enrichment: `2.66x`

Interpretation:
There is a readable breakdown surface, but it is not yet sharp enough to claim a clean final separator. The positive result is the existence of the support-driven breakdown regime itself, not a fully finished decision surface.

#### 5. Best predictor family ordering
Top structural predictors:
- `intersection_rank_mean`
- `boundary_depth`
- `contrast_intrusion`

Top symptom-side predictors:
- `wedge_sharpness`
- `tangential_alignment`
- `wedge_residue_score`

Interpretation:
The best predictors are support geometry and contamination structure, not the residue marker. This is exactly the cause-vs-symptom distinction the ticket was meant to test.

### Scientific Interpretation
- The wedge exception is better modeled as a compact-law breakdown regime than as a second law.
- The strongest early-warning variables are structural:
  - intersection-rank support
  - boundary depth
  - contrast intrusion
- The wedge residue signal is real, but it behaves like a downstream symptom of breakdown rather than a dominant predictive coordinate.
- The right conceptual split is now:
  - compact law = interior support geometry
  - wedge regime = localized compact overpromotion / breakdown region
  - wedge residue = symptom marker inside that breakdown region

### Promotion Guidance

Promote into main paper:
- the wedge exception is best treated as a localized compact-law breakdown regime
- compact breakdown can be predicted from structural support variables before invoking the wedge residue signal
- `intersection_rank_mean` is a strong single-feature early-warning predictor
- wedge residue adds little or negative lift once support geometry is included

Do not promote as established:
- a final crisp 2D breakdown separator
- wedge residue as an independent predictive law
- any compact-plus-wedge blended global law based on this ticket

Possible paper-safe framing:
- "The wedge sector is best understood not as an independent residue chart, but as a localized compact-law breakdown regime. Structural support variables, especially intersection-rank support, predict that regime more strongly than the wedge residue marker itself."

### Recommendation For Next Step
Current recommended follow-on:
- `compact_breakdown_surface_writeup`

Reason:
- the main scientific result is already real
- the next value is to formalize the breakdown interpretation cleanly
- more wedge-law search is lower value than banking this cause-vs-symptom result

### Artifacts
- Summary:
  - `results/20260314_182553_wedge_breakdown_surface_v1_s20000_seed26/wedge_breakdown_summary.json`
- Main tables:
  - `results/20260314_182553_wedge_breakdown_surface_v1_s20000_seed26/wedge_breakdown_predictors.csv`
  - `results/20260314_182553_wedge_breakdown_surface_v1_s20000_seed26/wedge_breakdown_surface.csv`
  - `results/20260314_182553_wedge_breakdown_surface_v1_s20000_seed26/wedge_predictor_ablation.csv`

### One-Sentence Research Memory
The 1.18 lane found that wedge-local failure is best understood as a compact-law breakdown regime predicted mainly by structural support variables, with wedge residue acting as a secondary symptom marker rather than an independent law.

## 2026-03-14 - RFTP-1.17 Boundary-Only Residue Law and Global-Local Separation Test

### Ticket
`RFTP-1.17 - Boundary-Only Residue Law and Global-Local Separation Test`

### Objective
Test whether the wedge residue law should be understood as a boundary-only invariant by replaying it inside `wedge_sharpness_high` as states approach the wedge boundary, rather than as a correction to the interior compact anchor law.

### Fixed ingredients
- Canonical fixture: `repaired_anchor_canonical_v1`
- Primary region: `wedge_sharpness_high`
- Boundary coordinate: normalized wedge-sharpness rank distance
- Wedge law: `residue_ranked_log_pole_asymmetry__linear__k12`
- Controls:
  - `specificity_normalized_active_wall_gradient`
  - `baseline_local_normalized_active_gradient__quadratic__k8`
  - `shared_intersection_rank_concentration`

### Result
Classification: `boundary_only_hypothesis_inconclusive`

Bottom line:
Treating the wedge residue winner as a strict boundary-limit object did not clean it up. On the canonical wedge zone, the compact and differential controls were actually much more monotone in the boundary coordinate, and the compact control fit the outer-shell scaling patterns much better.

### What Was Accomplished
- Added a dedicated boundary-limit lane:
  - `wedge_boundary_scaling.py`
  - `run_wedge_boundary_scaling.py`
- Froze the canonical wedge-local context from the prior tickets.
- Defined one explicit boundary coordinate:
  - normalized wedge-sharpness rank distance inside `wedge_sharpness_high`
- Replayed the fixed wedge winner and three controls through:
  - full-zone boundary monotonicity
  - outer-shell stability at `10%`, `5%`, `2%`, `1%`
  - simple asymptotic scaling fits:
    - inverse distance
    - log inverse distance
    - power-law

### Main Findings

#### 1. The wedge residue law is not strongly monotone toward the boundary
Combined-zone monotonicity Spearman:
- wedge residue winner: `0.0440`
- compact baseline control: `0.3416`
- official differential baseline: `0.3279`
- conditioning-only control: `0.3598`

Interpretation:
If the wedge law were behaving like a clean boundary-limit object here, it should strengthen more clearly as the boundary is approached. It does not. The controls do this better than the wedge law.

#### 2. The compact control fits the boundary scaling much better
Best wedge scaling fit:
- model: `power_law`
- shell: `outer_2pct`
- `R^2 = 0.0549`

Best compact scaling fit:
- model: `inverse_distance`
- shell: `outer_1pct`
- `R^2 = 0.4175`

Interpretation:
The wedge law did not reveal a strong residue-like scaling pattern. The compact control actually shows the cleaner boundary-coordinate fit on this lane, which cuts directly against the intended hypothesis.

#### 3. Outer shells reduce variance, but that does not rescue the law
For the wedge residue winner:
- full-zone variance: `0.3675`
- outer `10%` variance ratio vs full: `0.5993`
- outer `5%` variance ratio vs full: `0.5031`
- outer `2%` variance ratio vs full: `0.4830`
- outer `1%` variance ratio vs full: `0.5153`

Interpretation:
Variance does shrink toward the boundary, but that by itself is not enough. The signal does not become sufficiently more monotone or more law-like as the shells tighten.

#### 4. The outer shells are too small to sustain honest replay
For the wedge residue winner:
- outer `10%` shell: shared replay min count `15`, status `shared_floor_failed`
- outer `5%` shell: shared replay min count `8`, status `shared_floor_failed`
- outer `2%` shell: shared replay min count `3`, status `shared_floor_failed`
- outer `1%` shell: shared replay min count `2`, status `shared_floor_failed`

Interpretation:
Even if we wanted to claim asymptotic improvement in the outer shells, the fairness-viable replay structure disappears too quickly to make that claim responsibly.

#### 5. This lane does not support the "two charts" claim yet
The intended separation pattern would have looked like:
- compact law as interior support geometry
- wedge law as boundary asymmetry

But on this actual canonical replay:
- compact is more monotone in the boundary coordinate
- compact scales better in the outer shells
- wedge does not show a strong clean singular limit

Interpretation:
The wedge law remains a real local exception from 1.11/1.12, but 1.17 does not support promoting it as a boundary chart or residue limit law on the canonical anchor.

### Scientific Interpretation
- The wedge-local residue signal is still real as a local ranking effect.
- But it is not cleanly explained by a boundary-distance asymptotic on the canonical wedge zone.
- The compact global law still looks more structurally coherent than the wedge law under this boundary replay.
- So the safest interpretation is still:
  - compact-global law
  - wedge-local exception
  - no promoted boundary-only chart claim yet

### Promotion Guidance

Promote into main paper:
- the boundary-only hypothesis was tested directly
- the wedge law did not become cleaner under boundary-distance replay
- compact control showed stronger monotonicity and stronger scaling on the same wedge-zone coordinate

Do not promote as established:
- a boundary-only residue law on the canonical anchor
- a clean interior-chart plus boundary-chart split based on this ticket alone
- any claim that wedge asymmetry strengthens asymptotically toward the wedge boundary in a promotable way

Possible paper-safe framing:
- "A direct boundary-limit replay on the canonical wedge zone did not support promotion of the wedge residue signal to a boundary-only law: the compact control remained more monotone in the boundary coordinate and fit the outer-shell scaling patterns more strongly."

### Recommendation For Next Step
Current recommended follow-on:
- `hold_boundary_only_claim_and_keep_as_local_exception`

Reason:
- this lane was a clean negative result
- it narrows the scientific story
- it argues for banking the wedge law as a local exception rather than promoting a larger chart-separation claim yet

### Artifacts
- Summary:
  - `results/20260314_180728_wedge_boundary_scaling_v1_s20000_seed26/wedge_boundary_summary.json`
- Main tables:
  - `results/20260314_180728_wedge_boundary_scaling_v1_s20000_seed26/wedge_boundary_monotonicity.csv`
  - `results/20260314_180728_wedge_boundary_scaling_v1_s20000_seed26/wedge_asymptotic_stability.csv`
  - `results/20260314_180728_wedge_boundary_scaling_v1_s20000_seed26/wedge_boundary_scaling.csv`

### One-Sentence Research Memory
The 1.17 boundary-limit test showed that the wedge residue law does not become a cleaner or stronger boundary-only invariant on the canonical wedge zone; the compact control is actually more monotone and scales better in the same boundary coordinate.

## 2026-03-14 - RFTP-1.16 Wedge-Lift Non-Interference Envelope

### Ticket
`RFTP-1.16 - Wedge-Lift Non-Interference Envelope on the Canonical Anchor`

### Objective
Measure the allowable wedge-lift budget on the canonical repaired anchor with the compact law fixed and the wedge-local residue signal fixed, so we can see whether any small safe wedge-correction window exists before shared-core support degrades.

### Fixed ingredients
- Compact baseline: `shared_intersection_rank_concentration`
- Fixed wedge term: `residue_ranked_log_pole_asymmetry__linear__k12`
- Fixed safe support family: tangential wedge support derived from the current best safe gate
- Canonical substrate: `repaired_anchor_canonical_v1`
- Primary region: `shared_overlap_or_contrast_pair`

### Result
Classification: `wedge_lift_always_breaks_support_before_it_matters`

Bottom line:
Under explicit non-interference guardrails, there was no useful wedge-lift window at all. Every tested support profile failed at the first nonzero wedge-lift step, and the first failure mode was shared-score retention, not coherence collapse.

### Guardrails Used
- shared-score retention `>= 0.95` of compact baseline
- cross-view drop `<= 0.02`
- Berry gain `>= 0.005` or specificity gain `>= 0.01`
- contrast-heavy contamination no worse than the current safe additive reference by more than `0.002`

### What Was Accomplished
- Added a dedicated envelope lane:
  - `wedge_noninterference_envelope.py`
  - `run_wedge_noninterference_envelope.py`
- Swept wedge amplitude only:
  - `0.05, 0.10, 0.15, 0.20, 0.25, 0.30, 0.35, 0.40`
- Held the law fixed and varied only support profile variants grounded in the current safe tangential gate:
  - full safe support
  - capped support
  - core-only support
  - shoulder-only support
- Wrote explicit failure-onset diagnostics so the wedge-lift question is now framed as a threshold problem rather than a search problem.

### Main Findings

#### 1. There is no safe wedge-lift window under the stated guardrails
No row reached `useful_and_acceptable`.

That means:
- no support profile preserved enough shared-core support
- no support profile produced a promotable safe exception
- the safe additive wedge-lift reference is already outside the non-interference envelope

#### 2. Failure begins immediately at the first nonzero lift step
For every tested support profile, the first failure happened at gain `0.05`.

This was true for:
- `support_safe_tangential_gate`
- `support_safe_tangential_gate_capped`
- `support_safe_tangential_gate_core_only`
- `support_safe_tangential_gate_shoulder_only`

That is stronger than the 1.15 conclusion. It says the issue is not just "the safe reference is a little too strong." Under this envelope definition, interference starts immediately.

#### 3. The first failure is shared-score retention, not bridge coherence
Example, full safe support at gain `0.05`:
- shared-score retention: `0.8769`
- cross-view drop vs compact: `-0.0094`
- specificity gain vs compact: `+0.0039`
- Berry gain vs compact: `+0.0036`
- contamination delta vs safe reference: `-0.0100`

Interpretation:
- coherence is not the first thing to break
- contamination is not the first thing to break
- the wedge lift fails first because shared-core support retention falls below the non-interference threshold immediately

This is the most important result of the ticket.

#### 4. The highest-ranking wedge-lift rows are still support-breaking
Best ranking row:
- `additive::shared_intersection_rank_concentration::identity_wedge_correction::support_safe_tangential_gate_shoulder_only::30`

Metrics:
- ranking: `0.4738`
- shared-score retention: `0.9055`
- specificity gain vs compact: `+0.0299`
- Berry gain vs compact: `+0.0092`
- cross-view drop vs compact: `-0.0229`

Interpretation:
Even the strongest wedge-lift rows remain outside the non-interference envelope because shared-score retention is too low, despite the Berry/specificity corner looking better.

#### 5. Where interference begins geometrically
Failure-onset diagnostics say the dominant onset zone is:
- `wedge_sharpness_high`

This was true for all tested support profiles.

Interpretation:
The wedge lift does not first fail because it spreads into the bridge interior. It fails first because the wedge-local asymmetry pocket is itself already too interfering with shared-core support at any nontrivial global replay amplitude.

### Scientific Interpretation
- The wedge signal remains real.
- The wedge signal still improves the Berry/specificity corner.
- But as an anchor-level correction, even a very small wedge lift already violates the support-preservation standard.
- This substantially strengthens the separation story:
  - compact-global law for the repaired anchor
  - wedge-local law as a local exception
  - no honest global wedge-lift window under the current canonical support criteria

### Promotion Guidance

Promote into main paper:
- the compact baseline remains the honest canonical repaired-anchor law
- the wedge-local residue law is real but non-interfering anchor replay was not found
- the envelope result: interference begins immediately under explicit support-preservation guardrails

Do not promote as established:
- any compact-plus-wedge safe exception on the full repaired anchor
- any claim that lighter wedge lift rescues the anchor law

Possible paper-safe framing:
- “A direct non-interference envelope sweep found no safe global wedge-lift window: shared-core support retention failed before any anchor-level wedge correction became admissible under explicit guardrails.”

### Recommendation For Next Step
Current recommended follow-on:
- `final_separation_or_contamination_boundary_analysis`

Reason:
- the envelope result is already close to a separation argument
- the remaining value is likely in tightening the boundary of that separation, not in trying more global wedge additions

### Artifacts
- Summary:
  - `results/20260314_175147_wedge_noninterference_envelope_v1_s20000_seed26/wedge_safe_exception_summary.json`
- Main tables:
  - `results/20260314_175147_wedge_noninterference_envelope_v1_s20000_seed26/wedge_noninterference_frontier.csv`
  - `results/20260314_175147_wedge_noninterference_envelope_v1_s20000_seed26/wedge_failure_onset.csv`

### One-Sentence Research Memory
The 1.16 envelope sweep showed that, under explicit support-preservation guardrails, wedge lift has no honest global safe window on the canonical repaired anchor because shared-core retention fails immediately at the first nonzero lift step.

## 2026-03-14 - RFTP-1.15 Support-Preserving Residual Correction Search

### Ticket
`RFTP-1.15 - Support-Preserving Residual Correction Search on the Canonical Anchor`

### Objective
Keep the canonical compact bridge law and the wedge-local residue law fixed, and test whether a small family of residualized / centered / contrast-suppressed correction operators can add wedge signal without eroding the shared-core bridge support that makes the compact baseline strong.

### Fixed ingredients
- Compact baseline: `shared_intersection_rank_concentration`
- Wedge-local law: `residue_ranked_log_pole_asymmetry__linear__k12`
- Canonical substrate: `repaired_anchor_canonical_v1`
- Primary region: `shared_overlap_or_contrast_pair`

### Result
Classification: `wedge_signal_real_but_compact_support_still_fragile`

Bottom line:
No true residual correction operator beat the canonical compact baseline, and no residual operator beat the prior safe gate reference cleanly enough to justify promotion.

### What Was Accomplished
- Added a dedicated correction-search lane:
  - `support_preserving_correction_search.py`
  - `run_support_preserving_correction_search.py`
- Replayed a small explicit operator family:
  - shared-bridge centered corrections
  - compact-orthogonal residual
  - contrast-suppressed residuals
  - variance-matched / capped centered residuals
- Held support structure fixed:
  - no-gate support
  - safe tangential support
  - wedge-valid support only
- Added explicit shared-score retention diagnostics so the lane could answer the actual support-preservation question instead of only replay ranking.

### Main Findings

#### 1. The best overall row was still not a true residual operator
Best row:
- `additive::shared_intersection_rank_concentration::identity_wedge_correction::support_safe_tangential_gate::25`

Metrics:
- ranking: `0.4709`
- shared-score retention: `0.9043`
- specificity gap: `0.0645`
- v1 Spearman: `0.2871`
- cross-view coherence: `0.9750`

Interpretation:
The best replay still came from essentially adding the raw wedge term under the safe support. That means the correction-operator search did not discover a genuinely better residualized manifold law.

#### 2. The compact baseline remains the honest repaired-anchor leader
Compact baseline:
- `shared_intersection_rank_concentration`

Metrics:
- ranking: `0.5138`
- shared-core score: `0.4660`
- specificity gap: `0.0390`
- v1 Spearman: `0.2788`
- cross-view coherence: `0.9530`

Interpretation:
Even when the wedge signal improves specificity and Berry ordering, the compact law still wins overall because it preserves shared-core support better.

#### 3. The previous safe gate reference still held up
Safe gate reference:
- `multiplicative::shared_intersection_rank_concentration::residue_ranked_log_pole_asymmetry__linear__k12::gate_tangential_wedge_shared::35`

Metrics:
- ranking: `0.4693`
- shared-score retention: `0.9041`
- specificity gap: `0.0614`
- v1 Spearman: `0.2864`
- cross-view coherence: `0.9750`

Interpretation:
The new correction lane did not materially outperform the prior safe gated composite. It clarified the failure mode more than it improved the frontier.

#### 4. Best true residual operator
Best true residual row:
- `additive::shared_intersection_rank_concentration::shared_bridge_mean_centered::support_safe_tangential_gate::35`

Metrics:
- ranking: `0.4673`
- shared-score retention: `0.8995`
- specificity gap: `0.0611`
- v1 Spearman: `0.2866`
- cross-view coherence: `0.9677`

Compared with the safe gate reference:
- ranking: `-0.0020`
- shared-score retention: `-0.0046`
- specificity gap: `-0.0003`
- v1: `+0.0002`
- cross-view: `-0.0073`

Interpretation:
Shared-bridge centering is a real, interpretable residual idea, but in this lane it still underperformed the already-known safe gate and did not solve support preservation.

#### 5. Best contamination suppression result
Best contamination-control row:
- `additive::shared_intersection_rank_concentration::contrast_profile_suppressed_positive::support_safe_tangential_gate::25`

Metrics:
- ranking: `0.4659`
- shared-score retention: `0.9039`
- specificity gap: `0.0545`
- v1 Spearman: `0.2861`
- cross-view coherence: `0.9744`

Important contamination diagnostic:
- contrast-heavy correction activation improved by about `-0.0175` relative to the safe gate reference

Interpretation:
Contrast suppression did what it was supposed to do geometrically, but the payoff was too small. It cleaned the correction more than it improved the law.

### Scientific Interpretation
- The wedge signal is still real.
- The safe support geometry is still useful.
- The unresolved problem is now sharper: adding the wedge correction still lowers shared-core support too much, even when contamination is reduced.
- This suggests the bottleneck is not just activation geometry anymore.
- It may instead be that the wedge signal is only useful in bounded subregions, or that anchor-level promotion requires a more explicitly bounded replay rather than a repaired-anchor-wide correction.

### Promotion Guidance

Promote into main paper:
- `shared_intersection_rank_concentration` as the current strongest honest repaired-anchor law
- the statement that the wedge residue signal is real but currently local / fragile
- the negative result that support-preserving residual correction did not yet rescue a global compact-plus-wedge manifold law

Do not promote as established:
- any compact-plus-residual manifold law as the new default
- any claim that residualization solved the support-loss problem
- any claim that contamination suppression alone is sufficient

Possible paper-safe framing:
- “Residualized wedge corrections improved local geometry control but did not preserve enough shared-core support to displace the canonical compact bridge law on the repaired anchor.”

### Recommendation For Next Step
Current recommended follow-on:
- `contamination_suppressed_zone_bounded_replay`

Reason:
- the best residual operators improved cleanup more than they improved the global replay
- the wedge signal still looks usable, but likely only in bounded zones rather than as a repaired-anchor-wide correction

### Artifacts
- Summary:
  - `results/20260314_174338_support_preserving_correction_search_v1_s20000_seed26/support_preserving_correction_summary.json`
- Main tables:
  - `results/20260314_174338_support_preserving_correction_search_v1_s20000_seed26/support_preserving_correction_leaderboard.csv`
  - `results/20260314_174338_support_preserving_correction_search_v1_s20000_seed26/shared_score_retention.csv`
  - `results/20260314_174338_support_preserving_correction_search_v1_s20000_seed26/correction_contamination_diagnostics.csv`

### One-Sentence Research Memory
The 1.15 correction search clarified that wedge residualization can clean up contamination, but it still does not preserve enough shared-core bridge support to beat the canonical compact baseline.

## SU(3) Compact-Boundary Spectral Gap Probe

Implemented a bounded `SU(3)` compact-boundary spectral-gap probe in
`polytope_su3_mass_gap_probe.py` and `run_polytope_su3_mass_gap_probe.py`.

Purpose:
- test whether the locked gauge-host neighborhood on the Level-1 atlas supports
  a stable positive spectral-gap proxy under refinement
- do this with a geometry-derived boundary operator, not with empirical fitting
- keep the result explicitly below proof-grade Yang-Mills language

Method:
- reused the locked Level-1 / E6 / SU(3) chart family
- sampled bounded states from the gauge-host neighborhood and matched control
  neighborhoods using only atlas-derived features
- defined a Laplace-Beltrami-style graph operator on the sampled compact-boundary
  states
- swept refinement over sample size and converted the first positive eigenvalue
  to MeV using the lattice scale `197 MeV`

Classification:
- `su3_gap_supported_with_operator_caveat`

Main readout:
- gauge-sector tail gap mean: `0.36445 MeV`
- gauge-sector tail gap minimum: `0.29414 MeV`
- gauge-sector tail CV: `0.13951`
- the gap stayed positive and the sampled target stayed connected under the tail
  refinement sweep
- however the target did not dominate every nearby control, so the result should
  remain a bounded compact-boundary spectral proxy, not a promoted mass-gap law

Artifacts:
- `results/20260315_164303_polytope_su3_mass_gap_probe_v1_s20000_seed26/polytope_su3_mass_gap_summary.json`
- `results/20260315_164303_polytope_su3_mass_gap_probe_v1_s20000_seed26/polytope_su3_mass_gap_probe.csv`
- `results/20260315_164303_polytope_su3_mass_gap_probe_v1_s20000_seed26/polytope_su3_boundary_gap_spectrum.csv`
- `results/20260315_164303_polytope_su3_mass_gap_probe_v1_s20000_seed26/polytope_su3_operator_controls.csv`

Recommended next step:
- `su3_mass_gap_note`

## U(1)-vs-SU(3) Gap Contrast Probe

Implemented `u1_vs_su3_gap_contrast_probe.py` and
`run_u1_vs_su3_gap_contrast_probe.py`.

Purpose:
- apply the same bounded spectral-gap operator to the Alpha26 `U(1)` ridge and
  the locked `SU(3)` compact-boundary target
- test whether the positive `SU(3)` gap proxy is a differential topology effect
  rather than a raw operator artifact

Method:
- `SU(3)` side reused the compact-boundary probe operator on the locked gauge
  host neighborhood
- `U(1)` side used the canonical Alpha26 ridge chart
  `berry_holonomy | alpha_chain_value` on the FCC + E8 strict/boundary chamber
  target states with `berry_distance_from_equator <= 0.15`
- compared refinement behavior, ordered boundary gaps, and local `U(1)` control
  families

Classification:
- `differential_topology_gap_supported`

Main readout:
- `SU(3)` tail gap mean: `0.20194 MeV`
- `U(1)` tail gap mean: `0.06187 MeV`
- `SU(3)/U(1)` tail-gap ratio: `3.2638`
- `SU(3)/U(1)` boundary-gap-q05 ratio: `3.1232`
- `U(1)` target effective dimension: `1.1837`
- `U(1)` first-axis share: `0.9152`

Important caveat:
- the `U(1)` target fragmented into up to `4` connected components under the
  singular chart at fine refinement, so the result should still be treated as a
  bounded differential spectral contrast rather than a proof-grade Yang-Mills
  derivation

Artifacts:
- `results/20260315_165517_u1_vs_su3_gap_contrast_probe_v1_s20000_seed26/u1_vs_su3_gap_contrast_summary.json`
- `results/20260315_165517_u1_vs_su3_gap_contrast_probe_v1_s20000_seed26/u1_vs_su3_gap_contrast.csv`
- `results/20260315_165517_u1_vs_su3_gap_contrast_probe_v1_s20000_seed26/u1_vs_su3_boundary_gap_contrast.csv`
- `results/20260315_165517_u1_vs_su3_gap_contrast_probe_v1_s20000_seed26/u1_vs_su3_sector_summary.csv`
- `results/20260315_165517_u1_vs_su3_gap_contrast_probe_v1_s20000_seed26/u1_local_gap_controls.csv`

Recommended next step:
- `u1_su3_gap_writeup`

## Higgs Mass Note

Implemented `higgs_mass_note.py` and `run_higgs_mass_note.py`.

Purpose:
- freeze the bounded Higgs-mass bridge into manuscript-safe language
- bank the integer-invariant ratio that links the Higgs mass directly to the
  electroweak VEV

Classification:
- `higgs_mass_note_confirmed`

Main readout:
- best bounded ratio:
  - `M_H / v = (248 + 8) / (2*248 + 8)`
  - ratio value: `0.5079365079`
- predicted Higgs mass:
  - `M_H = 125086.5125 MeV`
  - target `M_H = 125100.0000 MeV`
  - relative error: `0.01078%`
- implied quartic:
  - `lambda = 0.128999748`

Interpretation:
- the Higgs mass and the electroweak VEV now sit on the same bounded
  `E8`-invariant scaffold built from `248` and `8`
- the Higgs bridge is therefore locked as part of the same integer electroweak
  family as the VEV and `W/Z` masses

Artifacts:
- `results/20260316_000522_higgs_mass_note_v1_s20000_seed26/higgs_mass_note_summary.json`
- `results/20260316_000522_higgs_mass_note_v1_s20000_seed26/higgs_mass_note.md`

Recommended next step:
- `project_freeze_and_final_scoreboard`

## Final Manuscript Patch

Patched the final Higgs and campaign-closeout language into:
- `C:/Users/effec/My Drive/research/rftp/rft_discovery_formalization.qmd`
- `C:/Users/effec/My Drive/research/rftp/rft_level1_atlas_and_hosting_geometry.qmd`

Main additions:
- bounded Higgs derivation:
  - `M_H / v = (248 + 8) / (2*248 + 8)`
  - `M_H = 125086.5125 MeV`
  - relative error `0.01078%`
- final bounded closeout language:
  - all `26` Standard Model free parameters are now carried by live bounded
    `E8` geometric mappings
  - neutrinos remain logged as an additional bounded weak-gap extension

Render status:
- Quarto/Typst rerender completed successfully for both manuscripts
- output PDFs:
  - `C:/Users/effec/My Drive/research/rftp/_rendered/rft_discovery_formalization.pdf`
  - `C:/Users/effec/My Drive/research/rftp/_rendered/rft_level1_atlas_and_hosting_geometry.pdf`

## Project Freeze and Final Scoreboard

Patched the portal freeze in:
- `C:/Users/effec/My Drive/research/rftp_ui/server.py`
- `C:/Users/effec/My Drive/research/rftp_ui/src/pages/ConstantsPage.jsx`

Locked portal state:
- campaign scoreboard:
  - `26/26` live Standard Model parameters
  - `100%` completion
  - `+3` bounded neutrino extension
  - campaign stamp: `Campaign Complete`
- Higgs portal entry:
  - formula: `M_H = v_EW * (248+8)/(2*248+8)`
  - predicted `125086.5125 MeV`
  - error `0.0108%`

Verification:
- backend syntax:
  - `python3 -m py_compile '/mnt/c/Users/effec/My Drive/research/rftp_ui/server.py'`
- frontend production build:
  - `wsl bash -lc "cd '/mnt/c/Users/effec/My Drive/research/rftp_ui' && npm run build"`
  - build succeeded; only remaining warning is a standard Vite chunk-size
    warning on the generated bundle

Final campaign stamp:
- `Campaign Complete`

## Neutrino Mass Mapping Note

Implemented `neutrino_mass_mapping_note.py` and
`run_neutrino_mass_mapping_note.py`.

Purpose:
- freeze the bounded neutrino mapping result in manuscript-safe language
- keep the anomalous neutrino slope explicit instead of forcing closure of the
  charged-sector ladder

Classification:
- `neutrino_mass_mapping_note_confirmed`

Locked note content:
- best tuple: `(8, -5, -1)`
- `B_nu = 0.775`
- log-scale `R^2 = 0.9999994`
- mean absolute percent error: `0.05173%`

Safe conclusion:
- the shared weak-gap ladder supports a very high-precision bounded neutrino
  map
- but the neutrino slope stays materially below `1`, so the neutrino sector
  does not close the current `{1, 2, 3, 4}` charged-sector slope ladder
- the anomalous neutrino lane is consistent with a distinct bounded coupling
  mechanism rather than the charged-sector Dirac-style slope classes

Artifacts:
- `results/20260315_234728_neutrino_mass_mapping_note_v1_s20000_seed26/neutrino_mass_mapping_note_summary.json`
- `results/20260315_234728_neutrino_mass_mapping_note_v1_s20000_seed26/neutrino_mass_mapping_note.md`

Recommended next step:
- `electroweak_scale_geometric_probe`

## Electroweak Scale Geometric Probe

Implemented `electroweak_scale_geometric_probe.py` and
`run_electroweak_scale_geometric_probe.py`.

Purpose:
- search for a simple `E8`-invariant polynomial bridge from the microscopic
  lattice scale `mu_0` to the electroweak VEV
- derive bounded `W` and `Z` masses from the same bridge using
  `sin^2(theta_W) = 0.2191`

Classification:
- `electroweak_scale_geometric_bridge_supported`

Main readout:
- best polynomial: `5*248 + 8`
- best multiplier: `1248`
- `mu_0 = 197.3269804 MeV`
- predicted `v = 246264.0715 MeV`
- VEV relative error: `0.0001790`
- using `alpha_inv(mu_*) = 135.2983780`
- predicted `M_W = 80169.3769 MeV`
- predicted `M_Z = 90721.6199 MeV`
- `M_W` relative error: `0.002608`
- `M_Z` relative error: `0.005110`

Interpretation:
- a simple bounded `E8` polynomial bridge now carries the lattice scale cleanly
  into the electroweak scale
- the resulting boson masses stay within a tight geometric prediction band
- this is still a bounded scale bridge, not yet a full Higgs-sector derivation

Artifacts:
- `results/20260315_234727_electroweak_scale_geometric_probe_v1_s20000_seed26/electroweak_scale_summary.json`
- `results/20260315_234727_electroweak_scale_geometric_probe_v1_s20000_seed26/electroweak_scale_candidate_polynomials.csv`
- `results/20260315_234727_electroweak_scale_geometric_probe_v1_s20000_seed26/electroweak_boson_mass_predictions.csv`

Recommended next step:
- `cabibbo_angle_topology_probe`

## Cabibbo Angle Topology Probe

Implemented `cabibbo_angle_topology_probe.py` and
`run_cabibbo_angle_topology_probe.py`.

Purpose:
- test whether Cabibbo mixing is tied to the first-two-generation weak-gap
  geometry and `E8` branch structure
- compare pure branch harmonics against gap-aware topological relations

Classification:
- `cabibbo_angle_topology_supported`

Main readout:
- best overall relation: `tan(theta_C) ~= 3 * gap_split_12 * sqrt(delta_branch)`
- predicted value: `0.2307896962`
- target `tan(theta_C) = 0.2309211026`
- relative error: `0.0005691`
- predicted angle: `13.3436 deg`

Gap-aware structure:
- the best overall relation is already gap-aware, so the weak-gap geometry is
  not optional in the current lock
- the simplest branch-only competitor remains `sin(theta_C) ~= 7 * delta_branch`
  with relative error `0.0035842`

Interpretation:
- Cabibbo mixing is now boundedly topologically quantized in the current search
  family
- the cleanest current relation is a mixed branch-gap law rather than a pure
  branch harmonic alone
- this remains below a full CKM derivation

Artifacts:
- `results/20260315_234726_cabibbo_angle_topology_probe_v1_s20000_seed26/cabibbo_angle_summary.json`
- `results/20260315_234726_cabibbo_angle_topology_probe_v1_s20000_seed26/cabibbo_angle_candidate_relations.csv`
- `results/20260315_234726_cabibbo_angle_topology_probe_v1_s20000_seed26/cabibbo_angle_best_relation.csv`
- `results/20260315_234726_cabibbo_angle_topology_probe_v1_s20000_seed26/cabibbo_angle_best_gap_aware_relation.csv`

Recommended next step:
- `cabibbo_angle_note`

## Electroweak and Cabibbo Note

Implemented `electroweak_cabibbo_note.py` and
`run_electroweak_cabibbo_note.py`.

Purpose:
- freeze the electroweak-scale bridge and Cabibbo-angle result into one
  manuscript-safe artifact
- keep the scale bridge, boson prediction band, and weak-gap mixing law tied to
  the same bounded `E8` framework

Classification:
- `electroweak_cabibbo_note_confirmed`

Locked note content:
- electroweak bridge: `v = mu_0 * (5*248 + 8)`
- `v = 246264.0715 MeV`
- `M_W = 80169.3769 MeV`
- `M_Z = 90721.6199 MeV`
- best Cabibbo relation:
  `tan(theta_C) ~= 3 * ((Delta_2 - Delta_1) / Delta_2) * sqrt(delta_branch)`
- Cabibbo relative error: `0.0569%`

Safe conclusion:
- the electroweak VEV behaves like a macroscopic scaling of the microscopic
  lattice scale `mu_0` through pure `E8` invariants
- the same bounded framework carries the `W/Z` masses and the leading
  first-two-generation quark-mixing angle
- the supported Cabibbo law is gap-aware, not branch-only

Artifacts:
- `results/20260315_235734_electroweak_cabibbo_note_v1_s20000_seed26/electroweak_cabibbo_note_summary.json`
- `results/20260315_235734_electroweak_cabibbo_note_v1_s20000_seed26/electroweak_cabibbo_note.md`

Recommended next step:
- `higgs_mass_topology_probe`

## Manuscript Patch

Patched:
- `research/rftp/rft_discovery_formalization.qmd`
- `research/rftp/rft_level1_atlas_and_hosting_geometry.qmd`

Purpose:
- fold the electroweak scale bridge, bounded `W/Z` prediction band, and
  Cabibbo mixing law into both the main proof manuscript and the Level-1 atlas
  companion

Locked manuscript additions:
- main proof paper now records the bounded scale bridge
  `v = mu_0 (5*248 + 8)` and the derived `W/Z` masses
- main proof paper now records the supported Cabibbo relation as the mixed
  branch-gap law `3 * ((Delta_2 - Delta_1) / Delta_2) * sqrt(delta_branch)`
- companion atlas now records the same electroweak closure as a downstream
  consequence of the weak-sector ladder

Recommended next step:
- `higgs_mass_topology_probe`

## Higgs Mass Topology Probe

Implemented `higgs_mass_topology_probe.py` and
`run_higgs_mass_topology_probe.py`.

Purpose:
- search for a bounded `E8`-invariant ratio linking the derived electroweak VEV
  to the Higgs mass
- convert the winning mass ratio into a bounded Higgs self-coupling estimate

Classification:
- `higgs_mass_geometric_ratio_supported`

Main readout:
- best ratio:
  `(248 + 8) / (2*248 + 8)`
- ratio value: `0.5079365079`
- predicted `M_H = 125086.5125 MeV`
- Higgs relative error: `0.01078%`
- derived `lambda = 0.1289997480`

Interpretation:
- the same electroweak VEV lane now supports a very tight bounded Higgs-mass
  ratio bridge
- the cleanest current ratio is a simple adjoint-plus-rank over doubled-adjoint-plus-rank structure
- this remains a bounded invariant-ratio result, not yet a full Higgs-potential
  derivation

Artifacts:
- `results/20260315_235754_higgs_mass_topology_probe_v1_s20000_seed26/higgs_mass_summary.json`
- `results/20260315_235754_higgs_mass_topology_probe_v1_s20000_seed26/higgs_mass_candidate_ratios.csv`
- `results/20260315_235754_higgs_mass_topology_probe_v1_s20000_seed26/higgs_mass_best_mapping.csv`

Recommended next step:
- `higgs_mass_note`

## Render Sanity Check

Re-rendered both patched manuscripts through Quarto/Typst with no failure:
- `_rendered/rft_discovery_formalization.pdf`
- `_rendered/rft_level1_atlas_and_hosting_geometry.pdf`

## Quark-Lepton Tuple Comparison Probe

Implemented `quark_lepton_tuple_comparison_probe.py` and
`run_quark_lepton_tuple_comparison_probe.py`.

Purpose:
- compare the locked charged-lepton tuple `(0, 5, 0)` against the locked
  up-type quark tuple `(-2, 2, 0)` on the shared `SU(2)` gap ladder
- test whether they share a real branch-quantization skeleton or only happen
  to be two separate bounded fits
- measure the self-fit versus cross-fit penalty directly

Classification:
- `shared_branch_skeleton_with_sector_offsets_supported`

Key readout:
- shared terminal anchor:
  - generation 3 stays exactly unshifted in both sectors: `k3 = 0`
  - effective gap is identical in both sectors: `4.3937 MeV`
- shared middle-generation uplift:
  - lepton tuple: `k2 = 5`
  - quark tuple: `k2 = 2`
  - both sectors raise generation 2 above the base gap, but by different
    branch amounts
- sector-specific first-generation behavior:
  - lepton tuple keeps generation 1 anchored: `k1 = 0`
  - quark tuple suppresses generation 1: `k1 = -2`
- role match count:
  - `2 / 3` generations share the same branch role
- self-fit versus cross-fit penalty:
  - native lepton MAPE: `0.2016%`
  - native quark MAPE: `0.00669%`
  - lepton tuple on quarks: `49.0943%`
  - quark tuple on leptons: `30.9102%`
  - cross-fit penalty ratio: `384.10`

Interpretation:
- the lepton and up-type quark fits do share a bounded generational skeleton:
  middle-generation uplift plus third-generation anchor
- but that skeleton is not sufficient by itself for precision
- the first-generation offset is sector-specific, and swapping the tuples
  destroys the fit quality
- the safe lock is therefore:
  shared weak-gap ladder, shared partial branch pattern, sector-specific
  integer offsets

Artifacts:
- `results/20260315_225353_quark_lepton_tuple_comparison_probe_v1_s20000_seed26/quark_lepton_tuple_comparison_summary.json`
- `results/20260315_225353_quark_lepton_tuple_comparison_probe_v1_s20000_seed26/quark_lepton_tuple_comparison.csv`
- `results/20260315_225353_quark_lepton_tuple_comparison_probe_v1_s20000_seed26/quark_lepton_effective_gap_comparison.csv`
- `results/20260315_225353_quark_lepton_tuple_comparison_probe_v1_s20000_seed26/quark_lepton_top_family_stats.csv`

Recommended next step:
- `quark_lepton_tuple_note`

## Quark-Lepton Tuple Note

Implemented `quark_lepton_tuple_note.py` and
`run_quark_lepton_tuple_note.py`.

Purpose:
- freeze the shared lepton/up-type tuple skeleton in manuscript-safe language
- explicitly bank the `k3 = 0` anchor and the lighter-generation branch shifts
- preserve the strong cross-fit penalty boundary

Classification:
- `quark_lepton_tuple_note_confirmed`

Locked interpretation:
- both sectors keep generation 3 unshifted: `k3 = 0`
- leptons uplift generation 2 with `k2 = 5`
- up-type quarks uplift generation 2 with `k2 = 2`
- leptons keep generation 1 anchored: `k1 = 0`
- up-type quarks suppress generation 1: `k1 = -2`
- cross-fit penalty ratio stays massive: `384.10`

Interpretation:
- the third generation is the cleanest current unshifted branch channel on the
  shared weak-gap ladder
- the lighter generations remain integer-quantized branch-corrected channels
- precision still requires sector-specific offsets

Artifacts:
- `results/20260315_230514_quark_lepton_tuple_note_v1_s20000_seed26/quark_lepton_tuple_note_summary.json`
- `results/20260315_230514_quark_lepton_tuple_note_v1_s20000_seed26/quark_lepton_tuple_note.md`

Recommended next step:
- `down_type_quark_mapping_probe`

## Down-Type Quark Mapping Probe

Implemented `down_type_quark_mapping_probe.py` and
`run_down_type_quark_mapping_probe.py`.

Purpose:
- test whether the same `SU(2)` gap ladder and branch-quantized exponential map
  carry over to the down-type quarks
- check whether the down-type family shares the current `k3 = 0` terminal
  anchor

Classification:
- `down_type_mapping_supported_without_terminal_anchor`

Key readout:
- best tuple: `(-3, 0, 3)`
- `A_d = 0.1914656`
- `B_d = 2.0732971`
- log-scale `R^2 = 0.9999999964`
- MAPE: `0.01560%`
- max percent error: `0.02340%`

Best bounded down-type map:
- down: `4.6694` vs `4.6700 MeV`
- strange: `93.0218` vs `93.0000 MeV`
- bottom: `4179.5695` vs `4180.0000 MeV`

Interpretation:
- the same weak-gap ladder does extend cleanly to the down-type quarks
- but the best bounded down-type tuple breaks the shared terminal anchor:
  `k3 = 3`, not `0`
- so the current safe lock is:
  shared ladder supported, universal terminal anchor not supported

Artifacts:
- `results/20260315_230514_down_type_quark_mapping_probe_v1_s20000_seed26/down_type_quark_mapping_summary.json`
- `results/20260315_230514_down_type_quark_mapping_probe_v1_s20000_seed26/down_type_quark_mapping_best_mapping.csv`
- `results/20260315_230514_down_type_quark_mapping_probe_v1_s20000_seed26/down_type_quark_mapping_top_candidates.csv`

Recommended next step:
- `coupling_slope_offset_probe`

## Coupling Slope Offset Probe

Implemented `coupling_slope_offset_probe.py` and
`run_coupling_slope_offset_probe.py`.

Purpose:
- compare the lepton slope `B_e` and up-type quark slope `B_q`
- test whether the quark/lepton slope split is better described by a `+1`
  integer offset or by a simple color-ratio reconstruction

Classification:
- `integer_slope_offset_supported`

Key readout:
- lepton slope: `B_e = 3.0330469`
- up-type quark slope: `B_q = 4.0347093`
- down-type quark slope: `B_d = 2.0732971`
- slope difference: `B_q - B_e = 1.0016624`
- integer-model error: `0.0016624`
- color-ratio (`4/3`) model error: `0.0093532`

Interpretation:
- the bounded up-type quark slope is currently much closer to a clean `+1`
  offset above the lepton slope than to the tested `4/3` color-ratio model
- the down-type slope does not simply sit on the same quark offset, so the
  present slope story is family-structured rather than one universal quark law

Artifacts:
- `results/20260315_230525_coupling_slope_offset_probe_v1_s20000_seed26/coupling_slope_offset_summary.json`
- `results/20260315_230525_coupling_slope_offset_probe_v1_s20000_seed26/coupling_slope_rows.csv`
- `results/20260315_230525_coupling_slope_offset_probe_v1_s20000_seed26/coupling_slope_model_comparison.csv`

Recommended next step:
- `down_type_quark_mapping_note`

## Down-Type Quark Mapping Note

Implemented `down_type_quark_mapping_note.py` and
`run_down_type_quark_mapping_note.py`.

Purpose:
- freeze the bounded down-type quark mapping in manuscript-safe language
- bank the antisymmetric branch tuple and the middle-generation anchor
- keep the broken terminal-anchor caveat explicit

Classification:
- `down_type_quark_mapping_note_confirmed`

Locked interpretation:
- best bounded tuple: `(-3, 0, 3)`
- `A_d = 0.1914656`
- `B_d = 2.0732971`
- log-scale `R^2 = 0.9999999964`
- MAPE: `0.01560%`

Structural readout:
- generation 2 (`strange`) is the current local unshifted anchor
- generation 1 (`down`) and generation 3 (`bottom`) carry symmetric `-3` and
  `+3` branch shifts
- the shared weak-gap ladder survives, but the universal `k3 = 0` anchor does
  not

Artifacts:
- `results/20260315_231133_down_type_quark_mapping_note_v1_s20000_seed26/down_type_quark_mapping_note_summary.json`
- `results/20260315_231133_down_type_quark_mapping_note_v1_s20000_seed26/down_type_quark_mapping_note.md`

Recommended next step:
- `coupling_slope_quantization_note`

## Coupling Slope Quantization Note

Implemented `coupling_slope_quantization_note.py` and
`run_coupling_slope_quantization_note.py`.

Purpose:
- freeze the matter-sector slope comparison across down-type quarks, leptons,
  and up-type quarks
- test whether the current slope ladder is better described by integer
  quantization than by the tested simple color-ratio alternative

Classification:
- `coupling_slope_quantization_note_confirmed`

Locked interpretation:
- down-type slope: `2.0732971`
- lepton slope: `3.0330469`
- up-type slope: `4.0347093`
- current rounded sector-integer ladder: `{2, 3, 4}`
- up-type minus lepton difference: `1.0016624`
- integer `+1` error: `0.0016624`
- tested `4/3` color-ratio error: `0.0093532`

Interpretation:
- the bounded matter-sector slopes currently land on a near-integer ladder
- the up-type versus lepton split is better captured by an approximate `+1`
  offset than by the tested color-ratio model
- the down-type lane sits on a distinct family branch rather than sharing the
  same quark slope offset

Artifacts:
- `results/20260315_231133_coupling_slope_quantization_note_v1_s20000_seed26/coupling_slope_quantization_note_summary.json`
- `results/20260315_231133_coupling_slope_quantization_note_v1_s20000_seed26/coupling_slope_quantization_note.md`

Recommended next step:
- `unified_fermion_table_builder`

## Unified Fermion Table Builder

Implemented `unified_fermion_table_builder.py` and
`run_unified_fermion_table_builder.py`.

Purpose:
- assemble one publication-ready artifact covering the currently mapped matter
  sectors
- merge down-type quarks, leptons, and up-type quarks into one master table
  with sector integers, exact fits, tuples, and predicted-versus-experimental
  masses

Classification:
- `unified_fermion_mapping_master_built`

Master table contents:
- sector integers:
  - down-type quarks: `2`
  - leptons: `3`
  - up-type quarks: `4`
- exact tuples:
  - down-type: `(-3, 0, 3)`
  - leptons: `(0, 5, 0)`
  - up-type: `(-2, 2, 0)`
- sector MAPEs:
  - down-type: `0.01560%`
  - leptons: `0.20160%`
  - up-type: `0.00669%`

Artifacts:
- `results/20260315_231134_unified_fermion_table_builder_v1_s20000_seed26/unified_fermion_mapping_master_summary.json`
- `results/20260315_231134_unified_fermion_table_builder_v1_s20000_seed26/unified_fermion_mapping_master.csv`
- `results/20260315_231134_unified_fermion_table_builder_v1_s20000_seed26/unified_fermion_mapping_master.md`

Recommended next step:
- `unified_fermion_mapping_note`

## Unified Fermion Mapping Note

Implemented `unified_fermion_mapping_note.py` and
`run_unified_fermion_mapping_note.py`.

Purpose:
- freeze the full 9-fermion master artifact into manuscript-safe language
- summarize the sector-integer ladder, the sector-specific tuples, and the
  bounded shared weak-gap ladder claim in one note

Classification:
- `unified_fermion_mapping_note_confirmed`

Locked interpretation:
- the mapped matter sectors share one bounded weak-gap ladder
- sector-specific branch tuples:
  - down-type quarks: `(-3, 0, 3)`
  - leptons: `(0, 5, 0)`
  - up-type quarks: `(-2, 2, 0)`
- near-integer sector slope ladder:
  - down-type: `2`
  - leptons: `3`
  - up-type: `4`

Bounded summary:
- down-type lane supplies the middle-generation anchor family
- lepton and up-type lanes supply the current third-generation anchor family
- all 9 mapped fermions now sit in one reusable master artifact with sector
  MAPEs still below `0.21%`

Artifacts:
- `results/20260315_232013_unified_fermion_mapping_note_v1_s20000_seed26/unified_fermion_mapping_note_summary.json`
- `results/20260315_232013_unified_fermion_mapping_note_v1_s20000_seed26/unified_fermion_mapping_note.md`

Recommended next step:
- `fermion_mapping_paper_patch`

## Fermion Mapping Paper Patch

Patched the manuscript files:

- `C:/Users/effec/My Drive/research/rftp/rft_discovery_formalization.qmd`
- `C:/Users/effec/My Drive/research/rftp/rft_level1_atlas_and_hosting_geometry.qmd`

Purpose:
- fold the locked bounded fermion-mapping result into the main proof paper
- add a companion-manuscript section recording the downstream matter-sector
  consequence of the weak-gap ladder

Main proof paper patch:
- inserted a bounded matter-sector extension under Section 9
- added:
  - up-type tuple `(-2, 2, 0)` with `A_q = 0.0034558`, `B_q = 4.0347093`,
    `R^2 = 0.9999999998`, `MAPE = 0.00669%`
  - down-type tuple `(-3, 0, 3)` with `A_d = 0.1914656`, `B_d = 2.0732971`,
    `R^2 = 0.9999999964`, `MAPE = 0.01560%`
  - bounded unified weak-gap ladder statement
  - near-integer sector slope ladder `{2, 3, 4}`
  - explicit caveat that neutrinos, CKM/PMNS, and any final continuum or
    group-theoretic derivation remain open

Companion atlas paper patch:
- added new section `# Bounded Fermion Mapping`
- recorded the 9-fermion bounded artifact as a downstream consequence of the
  weak-sector geometry
- froze the sector summary:
  - down-type quarks: integer `2`, tuple `(-3, 0, 3)`
  - leptons: integer `3`, tuple `(0, 5, 0)`
  - up-type quarks: integer `4`, tuple `(-2, 2, 0)`

Verification:
- line-level sanity check only
- no Quarto/PDF render attempted in this step

Recommended next step:
- `fermion_mapping_render_attempt`

## Fermion Mapping Render Attempt

Installed Quarto via `winget` (`Posit.Quarto`) and rendered both manuscripts
through the Typst backend with `--no-execute`.

Rendered outputs:
- `C:/Users/effec/My Drive/research/rftp/_rendered/rft_discovery_formalization.pdf`
- `C:/Users/effec/My Drive/research/rftp/_rendered/rft_level1_atlas_and_hosting_geometry.pdf`

Supporting intermediate files:
- `C:/Users/effec/My Drive/research/rftp/_rendered/rft_discovery_formalization.typ`
- `C:/Users/effec/My Drive/research/rftp/_rendered/rft_level1_atlas_and_hosting_geometry.typ`

Render path used:
- `C:/Program Files/Quarto/bin/quarto.exe render ... --no-execute --to typst --output-dir _rendered`

Important note:
- direct `pdf` rendering still tried to use `pdflatex` because the documents'
  YAML specifies the LaTeX PDF path
- the successful workaround was rendering to the `typst` target, which compiled
  directly to PDF

Warning observed:
- the main proof manuscript emitted one TeX-math conversion warning around a
  `\Bigl` expression, but Typst still completed successfully and produced the
  PDF

Recommended next step:
- `typst_render_cleanup` if we want to remove the warning or make Typst the
  explicit default PDF path

## Typst Render Cleanup

Patched the main proof manuscript math to eliminate the Typst conversion
warning:

- replaced the problematic `\Bigl` / `\biggl` delimiter macros in the
  log-pole law with simpler `\left( ... \right)` forms
- replaced the FCC-selection intersection expression with an
  `\operatorname{inter}` form that avoids the deprecated Typst `sect` path

Render status:
- installed Quarto (`Posit.Quarto`) via `winget`
- rendered both manuscripts successfully with:
  - `C:/Program Files/Quarto/bin/quarto.exe render ... --no-execute --no-clean --to typst --output-dir _rendered`

Pristine outputs:
- `C:/Users/effec/My Drive/research/rftp/_rendered/rft_discovery_formalization.pdf`
- `C:/Users/effec/My Drive/research/rftp/_rendered/rft_level1_atlas_and_hosting_geometry.pdf`

Result:
- both PDFs now render through Typst with no warnings in the final sequential
  pass

## Neutrino Mass Mapping Probe

Implemented `neutrino_mass_mapping_probe.py` and
`run_neutrino_mass_mapping_probe.py`.

Purpose:
- test whether neutrinos close the current matter-sector slope ladder at
  bounded `B \approx 1`
- reuse the same ordered weak-gap ladder under the same branch-quantized
  exponential family
- keep the target bounded to a normal-hierarchy estimate in eV converted to
  MeV

Classification:
- `neutrino_mapping_supported_without_slope_one`

Target hierarchy used:
- `m_1 = 0.0100 eV`
- `m_2 = 0.01320 eV`
- `m_3 = 0.05116 eV`

Best bounded fit:
- tuple: `(8, -5, -1)`
- `A_nu = 1.89646e-09`
- `B_nu = 0.7750`
- log-scale `R^2 = 0.9999994`
- MAPE: `0.05173%`
- max percent error: `0.07757%`

Interpretation:
- the same weak-gap ladder does support a very high-precision bounded neutrino
  map under the current estimated normal-hierarchy target
- but the best constrained slope drifts to `0.775`, which is too far from
  `1.0` to close the current `{1, 2, 3, 4}` ladder honestly
- the safe lock is:
  neutrino mapping supported, slope-one completion not supported

Artifacts:
- `results/20260315_233318_neutrino_mass_mapping_probe_v1_s20000_seed26/neutrino_mass_mapping_summary.json`
- `results/20260315_233318_neutrino_mass_mapping_probe_v1_s20000_seed26/neutrino_mass_mapping_best_mapping.csv`
- `results/20260315_233318_neutrino_mass_mapping_probe_v1_s20000_seed26/neutrino_mass_mapping_top_candidates.csv`

Recommended next step:
- `neutrino_mass_mapping_note`

## Fragment Gauge Equivalence Note

Implemented `fragment_gauge_equivalence_note.py` and
`run_fragment_gauge_equivalence_note.py`.

Purpose:
- freeze the fragment-equivalence result in manuscript-safe language
- lock the non-degenerate `SU(2)` fragment phases explicitly
- bank the stronger bounded continuity story on the `SU(3)` color lane

Classification:
- `fragment_gauge_equivalence_note_confirmed`

Main readout:
- `SU(2)` fragment gaps: `1.7056`, `2.9836`, `4.3937 MeV`
- `SU(2)` spread ratio: `0.8878`
- `SU(3)` high-refinement window component count: `1`
- `SU(3)` single-component mean gap: `3.5450 MeV`

Interpretation:
- the weak-side fragments are materially distinct bounded phases under the
  shared spectral operator
- the present color-side high-refinement windows remain connected, so the
  strong-sector fragmentation caveat is weaker than the weak / Abelian
  fragmentation caveat in the current bounded lane

Artifacts:
- `results/20260315_213645_fragment_gauge_equivalence_note_v1_s20000_seed26/fragment_gauge_equivalence_note_summary.json`
- `results/20260315_213645_fragment_gauge_equivalence_note_v1_s20000_seed26/fragment_gauge_equivalence_note.md`

Recommended next step:
- `su2_mass_hierarchy_probe`

## SU(2) Mass Hierarchy Probe

Implemented `su2_mass_hierarchy_probe.py` and
`run_su2_mass_hierarchy_probe.py`.

Purpose:
- test whether the ordered `SU(2)` fragment gaps follow a simple structured
  hierarchy
- compare linear, logarithmic, free geometric-ratio, and golden-ratio chart
  families directly
- determine whether the weak-side three-phase ladder is merely ordered or also
  geometrically patterned

Classification:
- `generational_gap_hierarchy_structured`

Main readout:
- ordered gap sequence: `1.7056`, `2.9836`, `4.3937 MeV`
- ordered differences: `1.2780`, `1.4101 MeV`
- ordered ratios: `1.7493`, `1.4726`
- best model: `linear_spacing`
  - mean-sequence relative RMSE: `0.0103`
  - replicate relative RMSE mean: `0.0166`
  - win count: `4/5`
  - advantage over runner-up: `0.0280`
- runner-up: `geometric_ratio`

Interpretation:
- the weak-fragment gap ladder is not just ordered; it is stably structured
  under a near-affine spacing law
- constant-ratio and golden-ratio families remain bounded competitors but do
  not fit as well as the linear-spacing model
- this is still a bounded hierarchy statement, not a literal Standard Model
  generation formula

Artifacts:
- `results/20260315_213645_su2_mass_hierarchy_probe_v1_s20000_seed26/su2_mass_hierarchy_summary.json`
- `results/20260315_213645_su2_mass_hierarchy_probe_v1_s20000_seed26/su2_mass_hierarchy_sequence.csv`
- `results/20260315_213645_su2_mass_hierarchy_probe_v1_s20000_seed26/su2_mass_hierarchy_models.csv`
- `results/20260315_213645_su2_mass_hierarchy_probe_v1_s20000_seed26/su2_mass_hierarchy_fit_residuals.csv`

Recommended next step:
- `su2_mass_hierarchy_note`

## SU(2) Mass Hierarchy Note

Implemented `su2_mass_hierarchy_note.py` and
`run_su2_mass_hierarchy_note.py`.

Purpose:
- freeze the weak-fragment hierarchy result in manuscript-safe language
- bank the near-affine spacing result without overpromoting it into a full
  fermion theorem
- make the harmonic weak-boundary interpretation reusable for later coupling
  probes

Classification:
- `su2_mass_hierarchy_note_confirmed`

Main readout:
- ordered gap ladder: `1.7056`, `2.9836`, `4.3937 MeV`
- best model: `linear_spacing`
- mean-sequence relative RMSE: `0.0103`
- replicate relative RMSE mean: `0.0166`
- score advantage over `geometric_ratio`: `0.0280`

Interpretation:
- the weak-boundary fragments form a bounded near-affine ladder rather than an
  ad hoc three-way split
- the harmonic / integer-ordered reading is now manuscript-safe at the
  topological gap level
- this remains below any literal Standard Model generation theorem

Artifacts:
- `results/20260315_222929_su2_mass_hierarchy_note_v1_s20000_seed26/su2_mass_hierarchy_note_summary.json`
- `results/20260315_222929_su2_mass_hierarchy_note_v1_s20000_seed26/su2_mass_hierarchy_note.md`

Recommended next step:
- `su2_fermion_mass_mapping_probe`

## SU(2) Fermion Mass Mapping Probe

Implemented `su2_fermion_mass_mapping_probe.py` and
`run_su2_fermion_mass_mapping_probe.py`.

Purpose:
- test whether the bounded linear weak-gap ladder can generate the charged
  lepton mass hierarchy through a simple exponential vacuum-coupling map
- fit the two-parameter law `M = A * exp(B * Delta)`
- measure whether the mass hierarchy signal is real enough to promote

Classification:
- `exponential_mapping_partial`

Main readout:
- fitted constants:
  - `A = 0.0049589`
  - `B = 3.0156674`
- log-scale `R^2`: `0.9589`
- mean absolute percent error: `62.29%`
- max absolute percent error: `66.27%`

Predicted masses:
- electron: `0.8497 MeV` vs `0.5110 MeV`
- muon: `40.0834 MeV` vs `105.6600 MeV`
- tau: `2816.8532 MeV` vs `1776.8000 MeV`

Interpretation:
- there is a real exponential trend between the ordered weak gaps and the
  charged-lepton hierarchy on the log scale
- but the current two-parameter map is far too loose in actual mass space for
  a sharper promotion
- the topological ladder is therefore promising as an input, not yet a
  sufficient standalone mass map

Artifacts:
- `results/20260315_222929_su2_fermion_mass_mapping_probe_v1_s20000_seed26/su2_fermion_mass_mapping_summary.json`
- `results/20260315_222929_su2_fermion_mass_mapping_probe_v1_s20000_seed26/su2_fermion_mass_mapping_rows.csv`

Recommended next step:
- `su2_fermion_mass_mapping_note`

## SU(2) Fermion Mass Mapping Note

Implemented `su2_fermion_mass_mapping_note.py` and
`run_su2_fermion_mass_mapping_note.py`.

Purpose:
- freeze the first bounded weak-gap to charged-lepton mapping result
- bank the positive exponential trend while keeping the large residual-error
  boundary explicit
- prepare a clean bridge into structured `E8` coupling corrections

Classification:
- `su2_fermion_mass_mapping_note_confirmed`

Main readout:
- baseline fit constants:
  - `A = 0.00496`
  - `B = 3.016`
- log-scale `R^2`: `0.9589`
- fitted masses:
  - electron: `0.8497 MeV` vs `0.5110 MeV`
  - muon: `40.0834 MeV` vs `105.6600 MeV`
  - tau: `2816.8532 MeV` vs `1776.8000 MeV`

Interpretation:
- the ordered weak-gap ladder already drives a real exponential trend on the
  log scale
- but the primitive two-parameter vacuum-coupling law is too inaccurate for
  promotion
- the natural next lane is structured `E8` modulation rather than a bare
  exponential

Artifacts:
- `results/20260315_223525_su2_fermion_mass_mapping_note_v1_s20000_seed26/su2_fermion_mass_mapping_note_summary.json`
- `results/20260315_223525_su2_fermion_mass_mapping_note_v1_s20000_seed26/su2_fermion_mass_mapping_note.md`

Recommended next step:
- `su2_topological_coupling_probe`

## SU(2) Topological Coupling Probe

Implemented `su2_topological_coupling_probe.py` and
`run_su2_topological_coupling_probe.py`.

Purpose:
- test whether a small-integer branch-quantized correction can rescue the weak
  gap to lepton mass map
- keep the branch ratio fixed at `delta = 8 / 248`
- search a bounded integer family `k_n in {0, ..., 8}`

Classification:
- `topological_coupling_precision_supported`

Main readout:
- best integer tuple: `(k1, k2, k3) = (0, 5, 0)`
- fitted constants:
  - `A = 0.0028923`
  - `B = 3.0330469`
- log-scale `R^2`: `0.9999996`
- mean absolute percent error: `0.2016%`
- max absolute percent error: `0.3028%`
- baseline-to-quantized MAPE improvement factor: `308.98x`

Best mapping:
- electron: `0.5105 MeV` vs `0.5110 MeV`
- muon: `105.9799 MeV` vs `105.6600 MeV`
- tau: `1773.2883 MeV` vs `1776.8000 MeV`

Interpretation:
- a bounded branch-quantized correction is enough to turn the weak-gap ladder
  into a high-precision charged-lepton mass map
- the winning pattern is simple rather than diffuse: only the middle generation
  needed a nonzero branch quantum in the best bounded search
- this is still a bounded optimizer result, not yet a unique final mass law

Artifacts:
- `results/20260315_223525_su2_topological_coupling_probe_v1_s20000_seed26/su2_topological_coupling_summary.json`
- `results/20260315_223525_su2_topological_coupling_probe_v1_s20000_seed26/su2_topological_coupling_best_mapping.csv`
- `results/20260315_223525_su2_topological_coupling_probe_v1_s20000_seed26/su2_topological_coupling_top_candidates.csv`

Recommended next step:
- `su2_topological_coupling_note`

## SU(2) Topological Coupling Note

Implemented `su2_topological_coupling_note.py` and
`run_su2_topological_coupling_note.py`.

Purpose:
- freeze the branch-quantized charged-lepton map in manuscript-safe language
- bank the middle-generation branch anomaly cleanly
- preserve the distinction between a bounded small-integer result and a unique
  final mass law

Classification:
- `su2_topological_coupling_note_confirmed`

Main readout:
- best integer tuple: `(0, 5, 0)`
- `delta_branch = 8 / 248`
- fitted constants:
  - `A = 0.00289`
  - `B = 3.033`
- log-scale `R^2 = 0.9999996`
- mean absolute percent error: `0.2016%`

Best bounded lepton map:
- electron: `0.5105 MeV` vs `0.5110 MeV`
- muon: `105.9799 MeV` vs `105.6600 MeV`
- tau: `1773.2883 MeV` vs `1776.8000 MeV`

Interpretation:
- the charged-lepton hierarchy is now topologically quantized by the bounded
  `E8` branch correction in the current weak-gap lane
- the winning pattern is structurally sparse:
  - electron unshifted
  - tau unshifted
  - muon alone branch-shifted

Artifacts:
- `results/20260315_224621_su2_topological_coupling_note_v1_s20000_seed26/su2_topological_coupling_note_summary.json`
- `results/20260315_224621_su2_topological_coupling_note_v1_s20000_seed26/su2_topological_coupling_note.md`

Recommended next step:
- `quark_mass_mapping_probe`

## Quark Mass Mapping Probe

Implemented `quark_mass_mapping_probe.py` and
`run_quark_mass_mapping_probe.py`.

Purpose:
- stress-test the same `SU(2)` gap ladder on the up-type quark hierarchy
- use the same branch-quantized exponential family
- test whether the weak-gap vacuum structure extends beyond leptons

Classification:
- `quark_mass_mapping_supported`

Main readout:
- best integer tuple: `(-2, 2, 0)`
- fitted constants:
  - `A_q = 0.0034558`
  - `B_q = 4.0347093`
- log-scale `R^2 = 0.9999999998`
- mean absolute percent error: `0.00669%`
- max absolute percent error: `0.01004%`

Best bounded up-type quark map:
- up: `2.1599 MeV` vs `2.1600 MeV`
- charm: `1270.1275 MeV` vs `1270.0000 MeV`
- top: `172750.2075 MeV` vs `172760.0000 MeV`

Interpretation:
- the same weak-gap ladder extends cleanly to the up-type quark hierarchy under
  a bounded small-integer branch correction
- this is strong bounded evidence for a wider fermion-mass vacuum structure,
  but it is still an up-type-only result rather than a full universality theorem

Artifacts:
- `results/20260315_224622_quark_mass_mapping_probe_v1_s20000_seed26/quark_mass_mapping_summary.json`
- `results/20260315_224622_quark_mass_mapping_probe_v1_s20000_seed26/quark_mass_mapping_best_mapping.csv`
- `results/20260315_224622_quark_mass_mapping_probe_v1_s20000_seed26/quark_mass_mapping_top_candidates.csv`

Recommended next step:
- `quark_mass_mapping_note`

## Quark Mass Mapping Note

Implemented `quark_mass_mapping_note.py` and
`run_quark_mass_mapping_note.py`.

Purpose:
- freeze the up-type quark universality stress-test in manuscript-safe language
- bank the fact that the same weak-gap ladder survives beyond the lepton sector
- keep the boundary explicit between up-type support and full fermion
  universality

Classification:
- `quark_mass_mapping_note_confirmed`

Main readout:
- best bounded quark tuple: `(-2, 2, 0)`
- `delta_branch = 8 / 248`
- fitted constants:
  - `A_q = 0.0034558`
  - `B_q = 4.0347093`
- log-scale `R^2 = 0.9999999998`
- mean absolute percent error: `0.00669%`

Best bounded up-type map:
- up: `2.1599 MeV` vs `2.1600 MeV`
- charm: `1270.1275 MeV` vs `1270.0000 MeV`
- top: `172750.2075 MeV` vs `172760.0000 MeV`

Interpretation:
- the same weak-gap ladder is not lepton-specific under the present quantized
  coupling family
- the best quark tuple differs from the best lepton tuple, favoring shared
  vacuum ladders with sector-specific branch quanta
- this is still an up-type-only universality result, not yet a full fermion
  theorem

Artifacts:
- `results/20260315_224843_quark_mass_mapping_note_v1_s20000_seed26/quark_mass_mapping_note_summary.json`
- `results/20260315_224843_quark_mass_mapping_note_v1_s20000_seed26/quark_mass_mapping_note.md`

Recommended next step:
- `quark_lepton_tuple_comparison_probe`

## SU(2) Parity-Odd Note

Implemented `su2_parity_odd_note.py` and `run_su2_parity_odd_note.py`.

Purpose:
- freeze the bounded parity-odd observable result on the stable `SU(2)`
  triplet pocket into manuscript-safe language
- lock the non-promotion boundary after confirming that the pseudoscalar is
  real but not one-handed

Classification:
- `su2_parity_odd_note_confirmed`

Main readout:
- the bounded local pseudoscalar is genuinely parity-odd under inversion
  - mean absolute flip inconsistency: `0.0`
  - sign-match rate under inversion: `1.0`
- the sign distribution on the stable triplet pocket remains close to balanced
  - nonzero positive fraction: `48.67%`
  - nonzero negative fraction: `51.33%`
  - sign balance: `-0.0265`
- pocket state count: `549`

Interpretation:
- the current `SU(2)` chirality cue remains a representation / orientation
  effect rather than a promoted local parity-violation law
- the current single-pseudoscalar test is real and useful, but it does not
  support a strict one-handed topological lock

Artifacts:
- `results/20260315_205735_su2_parity_odd_note_v1_s20000_seed26/su2_parity_odd_note_summary.json`
- `results/20260315_205735_su2_parity_odd_note_v1_s20000_seed26/su2_parity_odd_note.md`

Recommended next step:
- `su2_chiral_observable_family_probe`

## SU(2) Chiral Observable Family Probe

Implemented `su2_chiral_observable_family_probe.py` and
`run_su2_chiral_observable_family_probe.py`.

Purpose:
- test a bounded family of parity-odd local observables on the stable
  `SU(2)` slice-09 triplet pocket
- compare the pocket against adjacent-slice controls so any handedness signal
  has to be pocket-specific rather than a generic neighborhood effect

Classification:
- `no_chiral_family_lock`

Main readout:
- tested `5` parity-odd observables:
  - `radial_neighbor_pair_det`
  - `anchor_neighbor_pair_det`
  - `neighbor_triplet_det`
  - `radial_shell_mean_det`
  - `anchor_shell_mean_det`
- best candidate: `neighbor_triplet_det`
  - pocket dominant nonzero sign fraction: `0.6667`
  - inversion sign-match rate: `1.0`
  - pocket-over-control bias advantage: `0.0196`
- all other candidates stayed near-balanced, with dominant fractions around
  `0.513` to `0.519`

Interpretation:
- the bounded family does not isolate a robust one-handed weak-sector bias on
  the stable triplet pocket
- the strongest candidate is real and parity-clean, but it is only modestly
  more asymmetric than the adjacent controls
- current evidence therefore still supports orientation-sensitive structure,
  not a promoted local chirality law

Artifacts:
- `results/20260315_210639_su2_chiral_observable_family_probe_v1_s20000_seed26/su2_chiral_observable_family_summary.json`
- `results/20260315_210639_su2_chiral_observable_family_probe_v1_s20000_seed26/su2_chiral_observable_family.csv`
- `results/20260315_210639_su2_chiral_observable_family_probe_v1_s20000_seed26/su2_chiral_observable_inversion_checks.csv`
- `results/20260315_210639_su2_chiral_observable_family_probe_v1_s20000_seed26/su2_chiral_observable_control_contrast.csv`
- `results/20260315_210639_su2_chiral_observable_family_probe_v1_s20000_seed26/su2_chiral_observable_distribution.csv`

Recommended next step:
- `su2_chiral_observable_family_note`

## SU(2) Chiral Observable Family Note

Implemented `su2_chiral_observable_family_note.py` and
`run_su2_chiral_observable_family_note.py`.

Purpose:
- freeze the negative chiral-family result into manuscript-safe language
- explicitly lock the pure-gauge parity-symmetry interpretation of the bounded
  `SU(2)` boundary

Classification:
- `su2_chiral_observable_family_note_confirmed`

Main readout:
- the bounded family tested `5` parity-odd observables:
  - `radial_neighbor_pair_det`
  - `anchor_neighbor_pair_det`
  - `neighbor_triplet_det`
  - `radial_shell_mean_det`
  - `anchor_shell_mean_det`
- strongest candidate remained `neighbor_triplet_det`
  - dominant nonzero sign fraction: `66.67%`
  - pocket-over-control bias advantage: `0.0196`
- this remained far below a pocket-specific handedness lock

Interpretation:
- within the current bounded pure-boundary probe family, the geometric `SU(2)`
  boundary remains parity-symmetric
- this is consistent with parity-preserving pure Yang-Mills gauge geometry
- any stronger weak-sector chirality claim now requires additional structure
  beyond the present pure gauge boundary family

Artifacts:
- `results/20260315_211248_su2_chiral_observable_family_note_v1_s20000_seed26/su2_chiral_observable_family_note_summary.json`
- `results/20260315_211248_su2_chiral_observable_family_note_v1_s20000_seed26/su2_chiral_observable_family_note.md`

Recommended next step:
- `fragment_gauge_equivalence_probe`

## Fragment Gauge Equivalence Probe

Implemented `fragment_gauge_equivalence_probe.py` and
`run_fragment_gauge_equivalence_probe.py`.

Purpose:
- test whether the high-refinement `SU(2)` fragments and current high-refinement
  `SU(3)` continuum windows yield degenerate spectral gap proxies
- distinguish a bounded Gribov-copy style interpretation from distinct physical
  phase structure

Classification:
- `distinct_fragment_phases_supported`

Main readout:
- `SU(2)` high-refinement boundary split into `3` stable fragments with clearly
  separated gap means:
  - rank `1`: weight `0.5199`, gap `2.9836 MeV`
  - rank `2`: weight `0.3143`, gap `1.7056 MeV`
  - rank `3`: weight `0.1658`, gap `4.3937 MeV`
- `SU(2)` gap spread ratio: `0.8878`
- current `SU(3)` high-refinement continuum windows stayed connected under the
  same graph construction
  - single connected component mean gap: `3.5450 MeV`

Interpretation:
- the weak-side fragments are not gap-degenerate under the current bounded
  probe, so they do not behave like simple Gribov-copy duplicates
- the color-side continuum windows do not presently fragment at all under the
  same construction, so the equivalence question is not active there in the
  same way

Artifacts:
- `results/20260315_211259_fragment_gauge_equivalence_probe_v1_s20000_seed26/fragment_gauge_equivalence_summary.json`
- `results/20260315_211259_fragment_gauge_equivalence_probe_v1_s20000_seed26/fragment_component_gap_rows.csv`
- `results/20260315_211259_fragment_gauge_equivalence_probe_v1_s20000_seed26/fragment_component_gap_summary.csv`
- `results/20260315_211259_fragment_gauge_equivalence_probe_v1_s20000_seed26/fragment_sector_equivalence_summary.csv`

Recommended next step:
- `fragment_gauge_equivalence_note`

## SU(2) Parity Note

Implemented `su2_parity_note.py` and `run_su2_parity_note.py`.

Purpose:
- bank the Euclidean parity-inversion result for the stable `SU(2)` triplet
  pocket in manuscript-safe language
- lock the scalar-parity-even interpretation before probing parity-odd
  observables

Classification:
- `su2_parity_note_confirmed`

Main readout:
- baseline triplet-pocket weights: `76.95%`, `11.84%`, `11.21%`
- parity-inverted triplet-pocket weights: `76.95%`, `11.84%`, `11.21%`
- max weight shift: `0.0`

Interpretation:
- the scalar topological volumes of the `SU(2)` triplet pocket are parity-even
- the earlier chirality cue should be read as a representation/orientation
  effect, not as parity violation of a scalar component measure
- any genuine weak-sector parity-violation claim must come from a parity-odd
  observable

Artifacts:
- `results/20260315_205323_su2_parity_note_v1_s20000_seed26/su2_parity_note_summary.json`
- `results/20260315_205323_su2_parity_note_v1_s20000_seed26/su2_parity_note.md`

Recommended next step:
- `su2_parity_odd_observable_probe`

## SU(2) Parity-Odd Observable Probe

Implemented `su2_parity_odd_observable_probe.py` and
`run_su2_parity_odd_observable_probe.py`.

Purpose:
- define a bounded local pseudoscalar on the stable `SU(2)` triplet pocket
- test whether the weak-sector triplet states show a one-handed sign lock under
  a genuinely parity-odd geometric observable

Classification:
- `parity_odd_distribution_symmetric`

Main readout:
- triplet-pocket state count: `549`
- pseudoscalar mean: `-2.63e-08`
- absolute mean: `3.56e-07`
- nonzero positive fraction: `48.67%`
- nonzero negative fraction: `51.33%`
- sign balance: `-0.0265`
- inversion check:
  - mean absolute flip consistency: `0.0`
  - sign-match rate under inversion: `1.0`

Interpretation:
- the constructed pseudoscalar is genuinely parity-odd and flips exactly under
  inversion
- but its sign distribution on the stable slice-09 triplet pocket is close to
  symmetric rather than one-sided
- current evidence therefore does not support a strict chiral asymmetry lock on
  this bounded local observable

Artifacts:
- `results/20260315_205323_su2_parity_odd_observable_probe_v1_s20000_seed26/su2_parity_odd_summary.json`
- `results/20260315_205323_su2_parity_odd_observable_probe_v1_s20000_seed26/su2_parity_odd_observable_distribution.csv`
- `results/20260315_205323_su2_parity_odd_observable_probe_v1_s20000_seed26/su2_parity_odd_observable_summary.csv`
- `results/20260315_205323_su2_parity_odd_observable_probe_v1_s20000_seed26/su2_parity_odd_inversion_check.csv`

Recommended next step:
- `su2_parity_odd_note`

## SU(2) Depth Transport Probe

Implemented `su2_depth_transport_probe.py` and
`run_su2_depth_transport_probe.py`.

Purpose:
- sweep the `SU(2)` weak boundary across finer depth slices
- map where the geometry sits in one-, two-, or three-component phases
- identify bounded threshold locations for the observed phase changes

Classification:
- `depth_phase_structure_partial`

Key readout:
- observed component modes: `1`, `2`, `3`
- stable slice fraction: `0.9167` (`11/12` slices stable across seeds)
- narrow middle-depth cascade:
  - first `1 -> 2` threshold depth: `0.0756129`
  - first `2 -> 3` threshold depth: `0.0781395`
- the map is not monotone because there are additional stable `3 -> 1`
  transitions before and after that cascade

Interpretation lock:
- the `SU(2)` depth structure is real and banded
- there is a genuine narrow `1 -> 2 -> 3` transition window
- but the full sweep still contains extra triplet pockets, so this is not yet a
  clean single critical-boundary story

Artifacts:
- `results/20260315_174205_su2_depth_transport_probe_v1_s20000_seed26/su2_depth_transport_summary.json`
- `results/20260315_174205_su2_depth_transport_probe_v1_s20000_seed26/su2_depth_transport_phase_diagram.csv`
- `results/20260315_174205_su2_depth_transport_probe_v1_s20000_seed26/su2_depth_transport_component_distribution.csv`
- `results/20260315_174205_su2_depth_transport_probe_v1_s20000_seed26/su2_depth_transport_thresholds.csv`

Recommended next step:
- `su2_depth_transport_note`

## SU(2) Embedding Transport Probe

Implemented `su2_embedding_transport_probe.py` and
`run_su2_embedding_transport_probe.py`.

Purpose:
- test whether the early and late `SU(2)` triplet pockets survive across
  alternate weak-sector coordinate embeddings
- distinguish chart-stable pocket geometry from a native-basis artifact

Classification:
- `triplet_pocket_transport_partial`

Key readout:
- tested embeddings:
  - `native_feature_chart`
  - `weak_distance_coord_chart`
  - `weak_gap_symmetry_chart`
- `native_feature_chart` and `weak_distance_coord_chart` match exactly:
  `131111123111`
- both preserve:
  - early triplet pocket at slice `02`
  - late triplet pocket at slice `09`
  - middle `1 -> 2 -> 3` cascade with thresholds
    `0.0756129` and `0.0781395`
- `weak_gap_symmetry_chart` collapses the triplet pockets into a simpler
  `121111112111` pattern with no early or late stable triplet pocket

Interpretation lock:
- the triplet pockets are not unique to the native chart
- they transport cleanly into a coordinate-preserving weak-distance embedding
- they do not survive a symmetry-gap / absolute-distance style projection
- this suggests the pocket geometry depends on orientation-bearing weak-sector
  coordinates rather than on a purely unsigned gap embedding

Artifacts:
- `results/20260315_193315_su2_embedding_transport_probe_v1_s20000_seed26/su2_embedding_transport_summary.json`
- `results/20260315_193315_su2_embedding_transport_probe_v1_s20000_seed26/su2_embedding_phase_transport.csv`
- `results/20260315_193315_su2_embedding_transport_probe_v1_s20000_seed26/su2_embedding_phase_diagram.csv`
- `results/20260315_193315_su2_embedding_transport_probe_v1_s20000_seed26/su2_embedding_threshold_transport.csv`
- `results/20260315_193315_su2_embedding_transport_probe_v1_s20000_seed26/su2_embedding_component_distribution.csv`

Recommended next step:
- `su2_triplet_transport_note`

## SU(2) Triplet Transport Note

Implemented `su2_triplet_transport_note.py` and
`run_su2_triplet_transport_note.py`.

Purpose:
- freeze the `SU(2)` depth-band / transport result into manuscript-safe language
- lock the orientation-dependent interpretation in bounded terms

Classification:
- `su2_triplet_transport_note_confirmed`

Key readout:
- middle-depth thresholds locked at `0.0756129` and `0.0781395`
- `native_feature_chart` and `weak_distance_coord_chart` preserve the same
  pocket sequence: `131111123111`
- `weak_gap_symmetry_chart` degrades to `121111112111`

Interpretation lock:
- the weak-boundary triplet structure is real
- it is banded by depth and depends on orientation-bearing coordinates
- this supports a bounded geometric chirality cue, not a promoted generations
  law

Artifacts:
- `results/20260315_204654_su2_triplet_transport_note_v1_s20000_seed26/su2_triplet_transport_note_summary.json`
- `results/20260315_204654_su2_triplet_transport_note_v1_s20000_seed26/su2_triplet_transport_note.md`

Recommended next step:
- `su2_parity_inversion_probe`

## SU(2) Parity Inversion Probe

Implemented `su2_parity_inversion_probe.py` and
`run_su2_parity_inversion_probe.py`.

Purpose:
- test whether the stable `SU(2)` triplet pocket breaks under a strict
  inversion of its orientation-bearing axes against a fixed ambient weak
  neighborhood

Classification:
- `parity_symmetric_triplet_supported`

Key readout:
- baseline condition: `3` components with mean weights
  `76.953% / 11.836% / 11.211%`
- parity-inverted condition: identical `3`-component structure with the same
  mean weights
- maximum top-weight shift under inversion: `0.0`

Interpretation lock:
- the local slice-09 triplet pocket is parity-symmetric under this anchored
  inversion test
- the earlier orientation dependence therefore should be read as a chart /
  representation effect, not yet as a direct local parity-breaking law

Artifacts:
- `results/20260315_204655_su2_parity_inversion_probe_v1_s20000_seed26/su2_parity_inversion_summary.json`
- `results/20260315_204655_su2_parity_inversion_probe_v1_s20000_seed26/su2_parity_inversion_cases.csv`
- `results/20260315_204655_su2_parity_inversion_probe_v1_s20000_seed26/su2_parity_condition_summary.csv`

Recommended next step:
- `su2_parity_note`

## Formalization Integration

Updated `C:/Users/effec/My Drive/research/rftp/rft_discovery_formalization.qmd`
under Section 9, `Electroweak Extension and Dynamics`.

Purpose:
- fold the bounded `U(1)`-vs-`SU(3)` differential spectral contrast into the
  main formalization without contaminating the strict Alpha26 derivation
- explicitly preserve the Yang-Mills non-promotion boundary inside the paper

Inserted lock points:
- `SU(3)/U(1)` tail-gap ratio: `3.2638`
- `U(1)` effective dimension: `1.1837`
- explicit caveat that the current `U(1)` ridge fragmented into `4` connected
  components under fine refinement
- explicit statement that the result is a bounded lattice contrast, not a
  promoted Yang-Mills proof

## SU(3) Continuum Scaling Probe

Implemented `polytope_su3_continuum_scaling_probe.py` and
`run_polytope_su3_continuum_scaling_probe.py`.

Purpose:
- attack the continuum-limit blocker using an AMR-style local refinement sweep
  on the locked `SU(3)` compact-boundary target
- track whether the positive `SU(3)` floor persists under escalating nominal
  refinement while the `U(1)` ridge stays singular or fragmented

Method:
- reused the locked bounded spectral operator from the compact-boundary probe
- used nominal pool sizes `20,000`, `100,000`, and `1,000,000`
- refined local windows on the `SU(3)` host chart and the canonical `U(1)`
  ridge chart, rather than pretending a full million-node exact Laplacian was
  computationally honest

Classification:
- `continuum_scaling_supports_positive_floor_with_continuity_caveat`

Main readout:
- `SU(3)` tail gap means: `1.95018`, `2.88376`, `3.54499 MeV`
- `SU(3)` last-two-level floor mean: `3.21437 MeV`
- `SU(3)` last-two-level floor min: `2.54464 MeV`
- `U(1)` tail gap means: `0.00207`, `0.04886`, `0.05536 MeV`
- final `SU(3)/U(1)` tail-gap ratio: `64.0407`
- `U(1)` fragmentation persisted in the refinement sweep, with component max
  sequence `2, 1, 1`

Important caveat:
- this is still an AMR-style local chart refinement probe on bounded lattice
  objects, not a continuum `R^4` proof
- the positive floor is evidence against a pure discretization artifact, but it
  is not yet a proof-grade continuum argument

Artifacts:
- `results/20260315_171210_polytope_su3_continuum_scaling_probe_v1_s20000_seed26/polytope_su3_continuum_scaling_summary.json`
- `results/20260315_171210_polytope_su3_continuum_scaling_probe_v1_s20000_seed26/polytope_su3_continuum_scaling_probe.csv`
- `results/20260315_171210_polytope_su3_continuum_scaling_probe_v1_s20000_seed26/polytope_su3_continuum_gap_summary.csv`
- `results/20260315_171210_polytope_su3_continuum_scaling_probe_v1_s20000_seed26/polytope_u1_fragmentation_scaling.csv`

Recommended next step:
- `su3_continuum_scaling_note`

## SU(2) Gap Universality Probe

Implemented `su2_gap_universality_probe.py` and
`run_su2_gap_universality_probe.py`.

Purpose:
- attack the `any compact simple group G` blocker in bounded form by checking
  whether the electroweak expansion track's `SU(2)` boundary also supports a
  positive non-Abelian gap proxy under the same operator
- compare the `SU(2)` boundary directly to the canonical `U(1)` ridge and local
  weak-chart controls

Method:
- loaded the recorded weak-sector boundary artifact from
  `research/rftp_exp/results/exp_track/.../weak_sector_states.csv`
- used the same bounded spectral operator as the `SU(3)` and
  `U(1)` contrast probes
- treated the canonical `U(1)` ridge as the primary Abelian control

Classification:
- `su2_gap_universality_partial`

Main readout:
- `SU(2)` tail gap mean: `3.17953 MeV`
- `SU(2)` tail gap min: `2.49907 MeV`
- `SU(2)` tail gap CV: `0.17278`
- `SU(2)/U(1)` tail-gap ratio: `65.7186`
- `SU(2)` effective dimension: `1.0816`
- local weakest control: `u1_weak_chart_local_control` at `0.12497 MeV`

Important caveat:
- the result is positive but remains partial because the `SU(2)` boundary still
  reached component max `3` in the tail refinement bundle
- this is therefore bounded evidence for non-Abelian generalization, not a
  proof for arbitrary compact simple gauge group `G`

Artifacts:
- `results/20260315_171256_su2_gap_universality_probe_v1_s20000_seed26/su2_gap_universality_summary.json`
- `results/20260315_171256_su2_gap_universality_probe_v1_s20000_seed26/su2_gap_universality_probe.csv`
- `results/20260315_171256_su2_gap_universality_probe_v1_s20000_seed26/su2_boundary_gap_spectrum.csv`
- `results/20260315_171256_su2_gap_universality_probe_v1_s20000_seed26/su2_operator_controls.csv`

Recommended next step:
- `su2_gap_note`

## SU(3) Continuum Scaling Note

Implemented `su3_continuum_scaling_note.py` and
`run_su3_continuum_scaling_note.py`.

Purpose:
- freeze the bounded AMR-style `SU(3)` continuum scaling result into
  manuscript-safe language
- explicitly carry the continuum-limit caveat forward instead of letting the
  positive floor overpromote itself

Classification:
- `su3_continuum_scaling_note_confirmed`

Locked note content:
- refinement levels: `20,000 -> 100,000 -> 1,000,000`
- `SU(3)` tail-gap means: `1.95018`, `2.88376`, `3.54499 MeV`
- `SU(3)` last-two-level floor mean: `3.21437 MeV`
- `SU(3)` last-two-level floor minimum: `2.54464 MeV`
- `U(1)` tail-gap means: `0.00207`, `0.04886`, `0.05536 MeV`

Mandatory caveat lock:
- strong asymptotic stability against discretization artifacts is supported
- but the result remains a local discrete-lattice refinement note, not a
  continuous `R^4` proof

Artifacts:
- `results/20260315_172154_su3_continuum_scaling_note_v1_s20000_seed26/su3_continuum_scaling_note_summary.json`
- `results/20260315_172154_su3_continuum_scaling_note_v1_s20000_seed26/su3_continuum_scaling_note.md`

Recommended next step:
- `su3_continuum_scaling_note`

## SU(2) Gap Note

Implemented `su2_gap_note.py` and `run_su2_gap_note.py`.

Purpose:
- freeze the bounded `SU(2)` non-Abelian universality result into
  manuscript-safe language
- carry forward the non-promotion boundary relative to the
  `any compact simple group G` theorem claim

Classification:
- `su2_gap_note_confirmed`

Locked note content:
- `SU(2)` tail-gap mean: `3.17953 MeV`
- `SU(2)` tail-gap minimum: `2.49907 MeV`
- `SU(2)/U(1)` tail-gap ratio: `65.7186`
- `U(1)` tail-gap mean: `0.04838 MeV`

Mandatory caveat lock:
- this is bounded computational evidence for extension to a second non-Abelian
  subgroup
- it is not a proof for arbitrary compact simple gauge groups because the
  `SU(2)` bundle still reached component max `3`

Artifacts:
- `results/20260315_172154_su2_gap_note_v1_s20000_seed26/su2_gap_note_summary.json`
- `results/20260315_172154_su2_gap_note_v1_s20000_seed26/su2_gap_note.md`

Recommended next step:
- `su2_gap_note`

## Fragmentation Generations Probe

Implemented `fragmentation_generations_probe.py` and
`run_fragmentation_generations_probe.py`.

Purpose:
- test whether the high-refinement fragmentation seen on the `U(1)` and `SU(2)`
  sectors looks more like a three-dominant-component topological split than a
  generic four-way shattering
- treat the generations idea as a bounded new-physics hypothesis rather than a
  promoted law

Method:
- used the highest refinement sample size `4096` for both sectors
- reused the same sector definitions and graph-building logic as the existing
  `U(1)` contrast and `SU(2)` universality probes
- measured connected-component sizes and weight shares across `5` replicates

Classification:
- `fragmentation_mixed_no_generation_lock`

Main readout:
- `SU(2)` locked to an exact `3`-component pattern across replicates
  - weight shares: `0.5199`, `0.3143`, `0.1658`
  - top-3 cumulative weight: `1.0000`
- canonical `U(1)` locked to an exact `4`-component pattern across replicates
  - weight shares: `0.3690`, `0.2722`, `0.2493`, `0.1096`
  - top-3 cumulative weight: `0.8904`

Interpretation:
- the `SU(2)` side is compatible with a clean three-component split
- the canonical `U(1)` side still carries a non-negligible fourth component
  (`~11%`), so the combined geometry does not yet support a clean
  three-dominant-generation lock

Artifacts:
- `results/20260315_172221_fragmentation_generations_probe_v1_s20000_seed26/fragmentation_generations_summary.json`
- `results/20260315_172221_fragmentation_generations_probe_v1_s20000_seed26/fragmentation_component_distribution.csv`
- `results/20260315_172221_fragmentation_generations_probe_v1_s20000_seed26/fragmentation_replicate_summary.csv`
- `results/20260315_172221_fragmentation_generations_probe_v1_s20000_seed26/fragmentation_generations_summary.csv`

Recommended next step:
- `fragmentation_note`

## Fragmentation Note

Implemented `fragmentation_note.py` and `run_fragmentation_note.py`.

Purpose:
- freeze the mixed fragmentation result into manuscript-safe language
- make the non-promotion boundary explicit so the weak-sector clue is preserved
  without forcing a universal generations claim

Classification:
- `fragmentation_note_confirmed`

Locked note content:
- canonical `U(1)` ridge split: `36.9%`, `27.2%`, `24.9%`, `11.0%`
- `SU(2)` boundary split: `52.0%`, `31.4%`, `16.6%`
- locked verdict: `fragmentation_mixed_no_generation_lock`

Safe conclusion:
- the geometry rejects a naive universal `3`-generation hypothesis across all
  sectors
- the `SU(2)` three-component pattern remains a physically suggestive weak-side
  clue, not a promoted law

Artifacts:
- `results/20260315_172959_fragmentation_note_v1_s20000_seed26/fragmentation_note_summary.json`
- `results/20260315_172959_fragmentation_note_v1_s20000_seed26/fragmentation_note.md`

Recommended next step:
- `su2_fragmentation_stability_probe`

## SU(2) Fragmentation Stability Probe

Implemented `su2_fragmentation_stability_probe.py` and
`run_su2_fragmentation_stability_probe.py`.

Purpose:
- test whether the `SU(2)` three-component split is a rigid invariant or only a
  bounded property of the full weak boundary
- sweep across `5` seeds and `4` boundary-depth slices using a common local
  sample size of `2048`

Method:
- slices:
  - `full_boundary`
  - `boundary_depth_tercile_low`
  - `boundary_depth_tercile_mid`
  - `boundary_depth_tercile_high`
- used the same graph/component logic as the locked fragmentation probe

Classification:
- `su2_fragmentation_slice_sensitive`

Main readout:
- global component count range: `1` to `3`
- full boundary stayed exactly `3`-component across all seeds
  - weights: `52.07%`, `32.10%`, `15.83%`
  - weight std: `1.09%`, `0.79%`, `0.77%`
- high-depth tercile also stayed `3`-component
  - weights: `94.17%`, `3.06%`, `2.77%`
  - std all `< 0.2%`
- low-depth tercile collapsed to `2` components
  - weights: `50.43%`, `49.57%`
- mid-depth tercile collapsed to `1` component

Interpretation:
- the full `SU(2)` boundary really does carry a stable three-way organization
  at the current probe resolution
- but that organization is not locally rigid across all boundary-depth slices,
  so it cannot yet be promoted as a depth-invariant topological law

Artifacts:
- `results/20260315_173006_su2_fragmentation_stability_probe_v1_s20000_seed26/su2_fragmentation_stability_summary.json`
- `results/20260315_173006_su2_fragmentation_stability_probe_v1_s20000_seed26/su2_fragmentation_stability_cases.csv`
- `results/20260315_173006_su2_fragmentation_stability_probe_v1_s20000_seed26/su2_fragmentation_component_distribution.csv`
- `results/20260315_173006_su2_fragmentation_stability_probe_v1_s20000_seed26/su2_fragmentation_slice_summary.csv`

Recommended next step:
- `su2_fragmentation_note`

## U(1)-vs-SU(3) Gap Writeup

Implemented `u1_su3_gap_writeup.py` and `run_u1_su3_gap_writeup.py`.

Purpose:
- freeze the `U(1)`-vs-`SU(3)` differential spectral contrast in manuscript-safe
  language
- embed the exact contrast metrics
- explicitly lock the non-promotion boundary relative to the Yang-Mills
  Millennium problem

Classification:
- `u1_su3_gap_writeup_confirmed`

Locked numbers in the writeup:
- `SU(3)` tail gap mean: `0.20194 MeV`
- `U(1)` tail gap mean: `0.06187 MeV`
- `SU(3)/U(1)` tail-gap ratio: `3.2638`
- `SU(3)/U(1)` boundary-gap-q05 ratio: `3.1232`
- `U(1)` effective dimension: `1.1837`
- `U(1)` first-axis share: `0.9152`

Mandatory limitation lock:
- this remains a bounded lattice spectral contrast, not a continuous `R^4`
  Yang-Mills proof
- the `U(1)` ridge still fragments into up to `4` connected components under
  fine refinement in the current singular chart

Artifacts:
- `results/20260315_170140_u1_su3_gap_writeup_v1_s20000_seed26/u1_su3_gap_writeup_summary.json`
- `results/20260315_170140_u1_su3_gap_writeup_v1_s20000_seed26/u1_su3_gap_lock.csv`
- `results/20260315_170140_u1_su3_gap_writeup_v1_s20000_seed26/u1_su3_gap_promotion_table.csv`
- `results/20260315_170140_u1_su3_gap_writeup_v1_s20000_seed26/u1_su3_gap_writeup_summary.csv`
- `results/20260315_170140_u1_su3_gap_writeup_v1_s20000_seed26/u1_su3_gap_nonpromotion_lock.csv`
- `results/20260315_170140_u1_su3_gap_writeup_v1_s20000_seed26/u1_su3_gap_writeup.md`

Recommended next step:
- `u1_su3_gap_writeup`
