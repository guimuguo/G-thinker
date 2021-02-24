1. mc_run.cpp (MCF-I): original mcf program, with sequential 1st round split. no time delay divide conquer and no expand split. VNUM_ALLOWED_BEFORE_SPLIT is input argument
2. mc_tddq_run.cpp (MCF-S with fixed VNUM_ALLOWED_BEFORE_SPLIT): mcf program with sequential 1st round split and time delay divide conquer. no expand split
3. tddq_split_run.cpp (MCF-H with fixed VNUM_ALLOWED_BEFORE_SPLIT): mcf program with sequential 1st round split and time delay divide conquer and expand split. VNUM_ALLOWED_BEFORE_SPLIT 200000
4. tddq_seq_split_run.cpp (MCF-H): mcf program with sequential 1st round split and time delay divide conquer and expand split. VNUM_ALLOWED_BEFORE_SPLIT is input argument
5. tddq_para_split_run.cpp: mcf program with parallel 1st round split and time delay divide conquer and expand split. VNUM_ALLOWED_BEFORE_SPLIT is input argument; This method is not faster than sequential program (MCF-H). It will also easy to use up the memory when expand parameter go low.
6. tddq_non_expand_run.cpp (MCF-S): mcf program with sequential 1st round split and time delay divide conquer. No expand split. VNUM_ALLOWED_BEFORE_SPLIT is input argument
7. tddq_non_1split_run.cpp (MCF-C): mcf program with NO 1st round split. There is time delay divide conquer and expand split. 

we recommend tddq_split_run.cpp (MCF-H with fixed VNUM_ALLOWED_BEFORE_SPLIT).