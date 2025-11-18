# Whodunnit: **Pathosis Pseudocodexia**

A mysterious syndrome—*Pathosis Pseudocodexia*—is sweeping through our synthetic cohort. Clinical leads are nonexistent, so the entire investigation rests on you. We have expression profiles from matched control and affected samples, but there are no pre-cleared suspects. Any gene that survives your evidence gauntlet could be the culprit—just be prepared to defend your pick. And beware of red herrings: some genes shout loudly without actually driving the disease.

## Mission Checklist

1. **Interrogate Expression Data**  
   - Load the control vs. affected matrix.  
   - Compute log₂ fold changes, Welch t-tests, and BH-adjusted p-values.  
   - Rank genes strictly by differential expression and build your initial suspect pool.

2. **Map the Molecular Neighborhood**  
   - Query STRING-DB for the top DE genes to see which ones form dense interaction clusters versus loners.  
   - Capture quick network plots so you can reference how the suspects connect.

3. **Compare Sequence Evidence**  
   - Retrieve transcripts for the leading suspects (Entrez/BLAST).  
   - Scan for shared motifs or domains that might explain the phenotype.  
   - Optional: probe miRNA binding sites or methylation-sensitive regions if a shared motif emerges.

4. **Visualize Everything**  
   - Boxplots for whole datasets and filtered subsets.  
   - Tables/figures for DE rankings, motif counts, BLAST hits, and STRING clusters.  
   - Keep snapshots of each step so a reader can follow your logic—and so you can spot red herrings quickly.

5. **Stay Organized**  
   - Structure your notebook clearly (data loading → DE stats → network → sequence → conclusions).  
   - Use tidy variable names and explanatory comments to keep the workflow reproducible.

6. **Close the Case**  
   - Integrate expression, network context, and sequence motifs into a final suspicion narrative.  
   - Whether your trail leads to a well-known oncogene or an unexpected player, the verdict must rest on the evidence you assembled for *Pathosis Pseudocodexia*.

Happy sleuthing!
