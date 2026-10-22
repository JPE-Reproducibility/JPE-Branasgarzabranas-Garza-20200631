## Appendix: Detailed PII Detection Results

*Generated on 2026-10-22 10:08:08*

This appendix lists all detected instances of potential personally identifiable information (PII) in the project files. Each entry shows the matched PII terms and, for data files, sample values to help verify whether the flagged content is indeed sensitive.

### Full Summary Table

| File Type | File | Variables/References | PII Categories |
|-----------|------|----------------------|----------------|
| Data | `dataAG.csv` | 4 | loc, gender, birth |
| Data | `dataAL.csv` | 4 | loc, gender, birth |
| Data | `dataALsmall.csv` | 4 | loc, gender, birth |
| Data | `dataLL.csv` | 4 | loc, gender, birth |
| Data | `dataLLsmall.csv` | 4 | loc, gender, birth |
| Data | `dataME.csv` | 4 | loc, gender, birth |
| Data | `dataMEsmall.csv` | 4 | loc, gender, birth |
| Code | `Code.R` | 346 | name, lat, school, birth, gender, loc, location, coord, lname, son, second, child, block, lon |
| Code | `Table16.tex` | 1 | loc, location |
| Code | `Table17.tex` | 1 | loc, location |
| Code | `Table2.tex` | 1 | loc, location |
| Code | `Table20.tex` | 2 | lon |
| Code | `Table21.tex` | 2 | lon |
| Code | `Table3.tex` | 1 | loc, location |
| Code | `Table4.tex` | 1 | loc, location |
| Code | `revised ms.tex` | 36 | name, url, lat, lon, school, city, gender, loc, location, son, child, address, second, social, birth |
| Code | `summary_table.tex` | 2 | lat, school |
| Code | `table10.tex` | 1 | loc, location |
| Code | `table11.tex` | 1 | loc, location |
| Code | `table12.tex` | 1 | loc, location |
| Code | `table13.tex` | 1 | loc, location |
| Code | `table14.tex` | 3 | lat, school |
| Code | `table15.tex` | 3 | lat, school |
| Code | `table19.tex` | 1 | lat |
| Code | `table6.tex` | 1 | son |
| Code | `table9.tex` | 2 | gender, loc, location |

### Data Files

**/replication-package/Replication Package/data/dataAG.csv**

- Variable: `StartAlloc`
  - Matched terms: loc
  - Sample values: 62, 31
- Variable: `birthMonth`
  - Matched terms: birth
  - Sample values: Marzo, Agosto, Enero
- Variable: `birthYear`
  - Matched terms: birth
  - Sample values: 2012, 2011, 2010
- Variable: `gender`
  - Matched terms: gender
  - Sample values: F, M, Prefiero no especificarlo

**/replication-package/Replication Package/data/dataAL.csv**

- Variable: `StartAlloc`
  - Matched terms: loc
  - Sample values: 31, 62
- Variable: `birthMonth`
  - Matched terms: birth
  - Sample values: Marzo, Agosto, Octubre
- Variable: `birthYear`
  - Matched terms: birth
  - Sample values: 2005, 2006, 2004
- Variable: `gender`
  - Matched terms: gender
  - Sample values: M, F, Prefiero no especificarlo

**/replication-package/Replication Package/data/dataALsmall.csv**

- Variable: `StartAlloc`
  - Matched terms: loc
  - Sample values: 31, 62
- Variable: `birthMonth`
  - Matched terms: birth
  - Sample values: Mayo, Junio, Septiembre
- Variable: `birthYear`
  - Matched terms: birth
  - Sample values: 2016, 2015, 2014
- Variable: `gender`
  - Matched terms: gender
  - Sample values: M, F, Prefiero no especificarlo

**/replication-package/Replication Package/data/dataLL.csv**

- Variable: `StartAlloc`
  - Matched terms: loc
  - Sample values: 31, 62
- Variable: `birthMonth`
  - Matched terms: birth
  - Sample values: Junio, Agosto, Octubre
- Variable: `birthYear`
  - Matched terms: birth
  - Sample values: 2012, 2011, 2010
- Variable: `gender`
  - Matched terms: gender
  - Sample values: F, M, Prefiero no especificarlo

**/replication-package/Replication Package/data/dataLLsmall.csv**

- Variable: `StartAlloc`
  - Matched terms: loc
  - Sample values: 31, 62
- Variable: `birthMonth`
  - Matched terms: birth
  - Sample values: Mayo, Diciembre, Marzo
- Variable: `birthYear`
  - Matched terms: birth
  - Sample values: 2016, 2015, 2014
- Variable: `gender`
  - Matched terms: gender
  - Sample values: M, F, ni M, ni F

**/replication-package/Replication Package/data/dataME.csv**

- Variable: `StartAlloc`
  - Matched terms: loc
  - Sample values: 62, 31
- Variable: `birthMonth`
  - Matched terms: birth
  - Sample values: Agosto, Febrero, Octubre
- Variable: `birthYear`
  - Matched terms: birth
  - Sample values: 2006, 2005, 2004
- Variable: `gender`
  - Matched terms: gender
  - Sample values: F, M, Prefiero no especificarlo

**/replication-package/Replication Package/data/dataMEsmall.csv**

- Variable: `StartAlloc`
  - Matched terms: loc
  - Sample values: 31, 62
- Variable: `birthMonth`
  - Matched terms: birth
  - Sample values: Agosto, Octubre, Julio
- Variable: `birthYear`
  - Matched terms: birth
  - Sample values: 2016, 2015, 2014
- Variable: `gender`
  - Matched terms: gender
  - Sample values: F, M, ni M, ni F

### Code Files

**/replication-package/Replication Package/Code/Code.R**

- Line 36: name
  ```
  data = dataBig[,!(names(dataBig) %in% drop)]
  ```
- Line 69: lat
  ```
  grade == "4EPO" ~ "Late Elem.",
  ```
- Line 70: lat
  ```
  grade == "5EPO" ~ "Late Elem.",
  ```
- Line 71: lat
  ```
  grade == "6EPO" ~ "Late Elem.",
  ```
- Line 74: lat
  ```
  grade == "3ESO" ~ "Late Middle",
  ```
- Line 75: lat
  ```
  grade == "4ESO" ~ "Late Middle",
  ```
- Line 76: school
  ```
  grade == "1Bach" ~ "High School",
  ```
- Line 77: school
  ```
  grade == "2Bach" ~ "High School",
  ```
- Line 96: birth
  ```
  ## Birth Month
  ```
- Line 105: birth
  ```
  Month = month_mapping[birthMonth],
  ```
- Line 106: birth
  ```
  Year = as.numeric(as.character(birthYear)),
  ```
- Line 128: gender
  ```
  ## Gender Cleanup
  ```
- Line 130: gender
  ```
  filter(gender %in% c("M", "F")) %>%
  ```
- Line 131: gender
  ```
  mutate(gender = factor(gender))
  ```
- Line 133: lat
  ```
  ## Pay Calculation
  ```
- Line 136: loc
  ```
  PayWinner1 = ifelse(StartAlloc == 31, ToWinner1 + 3, ifelse(StartAlloc == 62, ToWinner1 + 6, NA)),
  ```
- Line 137: loc
  ```
  PayWinner2 = ifelse(StartAlloc == 31, ToWinner2 + 3, ifelse(StartAlloc == 62, ToWinner2 + 6, NA))
  ```
- Line 144: loc
  ```
  PayLoser1 = ifelse(StartAlloc == 31, 8-PayWinner1, ifelse(StartAlloc == 62, 8-PayWinner1, NA)),
  ```
- Line 145: loc
  ```
  PayLoser2 = ifelse(StartAlloc == 31, 8-PayWinner2, ifelse(StartAlloc == 62, 8-PayWinner2, NA))
  ```
- Line 156: loc
  ```
  data$ToWinner1Type[data$StartAlloc==31 & data$ToWinner1==2]<-"1-Soc"
  ```
- Line 157: loc
  ```
  data$ToWinner1Type[data$StartAlloc==31 & data$ToWinner1==3]<-"2-Rep"
  ```
- Line 158: loc
  ```
  data$ToWinner1Type[data$StartAlloc==31 & data$ToWinner1==1]<-"3-Comm"
  ```
- Line 160: loc
  ```
  data$ToWinner1Type[data$StartAlloc==62 & data$ToWinner1==-2]<-"3-Comm"
  ```
- Line 161: loc
  ```
  data$ToWinner1Type[data$StartAlloc==62 & data$ToWinner1==0]<-"2-Rep"
  ```
- Line 162: loc
  ```
  data$ToWinner1Type[data$StartAlloc==62 & data$ToWinner1==-1]<-"1-Soc"
  ```
- Line 165: loc
  ```
  data$ToWinner2Type[data$StartAlloc==31 & data$ToWinner2==2]<-"1-Soc"
  ```
- Line 166: loc
  ```
  data$ToWinner2Type[data$StartAlloc==31 & data$ToWinner2==3]<-"2-Rep"
  ```
- Line 167: loc
  ```
  data$ToWinner2Type[data$StartAlloc==31 & data$ToWinner2==1]<-"3-Comm"
  ```
- Line 169: loc
  ```
  data$ToWinner2Type[data$StartAlloc==62 & data$ToWinner2==-2]<-"3-Comm"
  ```
- Line 170: loc
  ```
  data$ToWinner2Type[data$StartAlloc==62 & data$ToWinner2==0]<-"2-Rep"
  ```
- Line 171: loc
  ```
  data$ToWinner2Type[data$StartAlloc==62 & data$ToWinner2==-1]<-"1-Soc"
  ```
- Line 192: loc
  ```
  data$Cond[data$StartAlloc=="62" & data$Treatment=="questions"]<-"Talent62"
  ```
- Line 193: loc
  ```
  data$Cond[data$StartAlloc=="62" & data$Treatment=="luck"]<-"Luck62"
  ```
- Line 194: loc
  ```
  data$Cond[data$StartAlloc=="62" & data$Treatment=="sliders"]<-"Effort62"
  ```
- Line 196: loc
  ```
  data$Cond[data$StartAlloc=="31" & data$Treatment=="questions"]<-"Talent31"
  ```
- Line 197: loc
  ```
  data$Cond[data$StartAlloc=="31" & data$Treatment=="luck"]<-"Luck31"
  ```
- Line 198: loc
  ```
  data$Cond[data$StartAlloc=="31" & data$Treatment=="sliders"]<-"Effort31"
  ```
- Line 204: gender
  ```
  keep1<-c("Campus","SessionCode","ClientID","BigPic1","BigPic2","BigPic3","BigPic4","BigPic5","gender
  ```
- Line 206: gender
  ```
  keep2<-c("Campus","SessionCode","ClientID","BigPic1","BigPic2","BigPic3","BigPic4","BigPic5","Q1","Q
  ```
- Line 219: loc
  ```
  table(data$grade1,data$Treatment,data$StartAlloc)
  ```
- Line 231: loc, location
  ```
  # Initial allocation: drop addition rows with no recorded initial choice.
  ```
- Line 232: loc, location
  ```
  # Final allocation:   drop addition rows with no recorded final choice.
  ```
- Line 233: loc
  ```
  df1 <- subset(data, Age < 225 & (StartAlloc == 62 | (StartAlloc == 31 & ToWinner1 != 0)))
  ```
- Line 234: loc
  ```
  df2 <- subset(data, Age < 225 & (StartAlloc == 62 | (StartAlloc == 31 & ToWinner2 != 0)))
  ```
- Line 238: gender, loc
  ```
  "Age + Treatment + as.factor(StartAlloc) + gender + Siblings + Topic",
  ```
- Line 239: gender, loc
  ```
  "Age + Treatment * as.factor(StartAlloc) + gender + Siblings + Topic",
  ```
- Line 240: gender, loc
  ```
  "Age + I(Age^2) + Treatment + as.factor(StartAlloc) + gender + Siblings + Topic",
  ```
- Line 241: gender, loc
  ```
  "Age + I(Age^2) + Treatment * as.factor(StartAlloc) + gender + Siblings + Topic"
  ```
- Line 255: loc
  ```
  "^as\\.factor\\(StartAlloc\\)62$"                    = "\\textit{redist.}",
  ```
- Line 256: gender
  ```
  "^gender"                                            = "\\textit{Male}",
  ```
- Line 259: loc
  ```
  "^Treatmentquestions:as\\.factor\\(StartAlloc\\)62$" = "\\textit{redist.}$\\times$\\textit{talent}",
  ```
- Line 260: loc
  ```
  "^Treatmentsliders:as\\.factor\\(StartAlloc\\)62$"   = "\\textit{redist.}$\\times$\\textit{effort}"
  ```
- Line 266: name
  ```
  old <- rownames(ct)
  ```
- Line 268: name
  ```
  for (p in names(labels)) new[grepl(p, old)] <- labels[[p]]
  ```
- Line 270: name
  ```
  coef.names  = new,
  ```
- Line 271: name
  ```
  coef        = unname(ct[, "Estimate"]),
  ```
- Line 272: name
  ```
  se          = unname(ct[, "Std. Error"]),
  ```
- Line 273: name
  ```
  pvalues     = unname(ct[, "Pr(>|t|)"]),
  ```
- Line 274: name
  ```
  gof.names   = c("Num. obs.", "R$^2$", "Adj. R$^2$"),
  ```
- Line 275: name
  ```
  gof         = c(nobs(m), unname(r2(m, "r2")), unname(r2(m, "ar2"))),
  ```
- Line 293: name
  ```
  custom.model.names = c(rep("Initial", 4), rep("Final", 4)),
  ```
- Line 294: name
  ```
  custom.coef.map    = as.list(setNames(unname(labels), unname(labels))),
  ```
- Line 303: loc, location
  ```
  caption            = "Main treatment effects in the \\textit{initial} and \\textit{final} allocation
  ```
- Line 325: loc
  ```
  graph <- ddply(data,c("StartAlloc"),summarise,
  ```
- Line 329: loc
  ```
  graph$StartAlloc <- factor(graph$StartAlloc, levels = c("62", "31"))
  ```
- Line 331: loc
  ```
  g <- ggplot(graph, aes(y = as.numeric(mean), x = StartAlloc)) +
  ```
- Line 333: coord
  ```
  coord_cartesian(ylim = c(2, 4)) +
  ```
- Line 358: loc
  ```
  t.test(subset(data,StartAlloc==31 & ToWinner1!=0)$PayWinner1,subset(data,StartAlloc==62)$PayWinner1)
  ```
- Line 376: coord
  ```
  coord_cartesian(ylim = c(2, 4)) +
  ```
- Line 407: loc
  ```
  graph <- ddply(data,c("StartAlloc"),summarise,
  ```
- Line 411: loc
  ```
  graph$StartAlloc <- factor(graph$StartAlloc, levels = c("62", "31"))
  ```
- Line 413: loc
  ```
  g <- ggplot(graph, aes(y = as.numeric(mean), x = as.factor(StartAlloc))) +
  ```
- Line 415: coord
  ```
  coord_cartesian(ylim = c(2, 4)) +
  ```
- Line 439: loc
  ```
  t.test(subset(data,StartAlloc==31)$PayWinner2,subset(data,StartAlloc==62)$PayWinner2)
  ```
- Line 453: coord
  ```
  coord_cartesian(ylim = c(2, 4)) +
  ```
- Line 499: lat
  ```
  # Row labels, in the order of the table. Later patterns override earlier ones.
  ```
- Line 505: gender
  ```
  "^gender"                                            = "\\textit{Male}",
  ```
- Line 508: loc
  ```
  "^as\\.factor\\(StartAlloc\\)62$"                    = "\\textit{redist.}",
  ```
- Line 509: loc
  ```
  "^Age:as\\.factor\\(StartAlloc\\)62$|^as\\.factor\\(StartAlloc\\)62:Age$" =
  ```
- Line 511: loc
  ```
  "StartAlloc.*Age\\^2|Age\\^2.*StartAlloc"            = "\\textit{Age}$^2\\times$\\textit{redist.}"
  ```
- Line 517: name
  ```
  old <- rownames(ct)
  ```
- Line 519: name
  ```
  for (p in names(labels)) new[grepl(p, old)] <- labels[[p]]
  ```
- Line 521: name
  ```
  coef.names  = new,
  ```
- Line 522: name
  ```
  coef        = unname(ct[, "Estimate"]),
  ```
- Line 523: name
  ```
  se          = unname(ct[, "Std. Error"]),
  ```
- Line 524: name
  ```
  pvalues     = unname(ct[, "Pr(>|t|)"]),
  ```
- Line 525: name
  ```
  gof.names   = c("Num. obs.", "Num. groups FE", "Num. clusters SE", "R$^2$", "Adj. R$^2$"),
  ```
- Line 527: name
  ```
  unname(m$fixef_sizes[1]),
  ```
- Line 529: name
  ```
  unname(r2(m, "r2")), unname(r2(m, "ar2"))),
  ```
- Line 536: loc, location
  ```
  # decision = 1 for the initial allocation, 2 for the final allocation.
  ```
- Line 540: loc
  ```
  d62  <- data[data$Age < 225 & data$StartAlloc == 62, ]
  ```
- Line 541: loc
  ```
  d31  <- data[data$Age < 225 & data$StartAlloc == 31 & rec, ]
  ```
- Line 544: gender
  ```
  ctrl <- "Treatment + gender + Siblings + Topic"
  ```
- Line 553: loc
  ```
  list("Age * as.factor(StartAlloc)",                                     dall),
  ```
- Line 554: loc
  ```
  list("Age * as.factor(StartAlloc) + I(Age^2) * as.factor(StartAlloc)",  dall)
  ```
- Line 561: name
  ```
  custom.model.names = c("Redistribution", "Redistribution", "Addition", "Addition", "All", "All"),
  ```
- Line 562: name
  ```
  custom.coef.map    = as.list(setNames(unname(labels), unname(labels))),
  ```
- Line 580: loc, location
  ```
  "\\textit{Initial} allocation to the loser by treatments and age",
  ```
- Line 583: loc, location
  ```
  "\\textit{Final} allocation to the loser by treatments and age",
  ```
- Line 592: loc, location
  ```
  # Quadratic best fit of the allocation to the loser on age, by winner selection
  ```
- Line 595: loc, location
  ```
  # decision = 1 (initial allocation, Figure 5) or 2 (final allocation, Figure 6).
  ```
- Line 600: loc
  ```
  d <- if (env == 62) data[data$Age < 225 & data$StartAlloc == 62, ] else
  ```
- Line 601: loc
  ```
  data[data$Age < 225 & data$StartAlloc == 31 & rec, ]
  ```
- Line 602: name
  ```
  d$loser <- 8 - pay[as.integer(rownames(d))]
  ```
- Line 607: lname, name
  ```
  colnames(out) <- c("X", "age", "Treatment", "predic")
  ```
- Line 629: name
  ```
  "Talent" = "gold"), name = " ") +
  ```
- Line 662: lname, name
  ```
  Y <- sapply(colnames(P), function(k) as.numeric(Y == k))
  ```
- Line 663: name
  ```
  cls <- rownames(coef(x))                       # non-baseline classes
  ```
- Line 665: lname, name
  ```
  colnames(S) <- as.vector(t(outer(cls, colnames(X), paste, sep = ":")))
  ```
- Line 673: son
  ```
  # in the Poisson columns as in the original code
  ```
- Line 687: loc
  ```
  base62 <- with(data, Age < 225 & Treatment != "luck" & StartAlloc == 62)
  ```
- Line 688: loc
  ```
  base31 <- with(data, Age < 225 & Treatment != "luck" & StartAlloc == 31 &
  ```
- Line 692: gender
  ```
  ctrl   <- "gender + Siblings + Topic + Treatment + howHard5 + howWell5"
  ```
- Line 695: son
  ```
  rhs_p  <- if (age_unit == "years") rhs_y else rhs_m   # Poisson columns
  ```
- Line 697: son
  ```
  # Poisson column: coefficients, two-way clustered SE (session, campus)
  ```
- Line 699: son
  ```
  m <- glm(as.formula(paste(lhs, "~", rhs_p)), family = poisson, data = d)
  ```
- Line 710: name
  ```
  cl <- d[rownames(mf), cluster_vars, drop = FALSE]
  ```
- Line 713: lname, name
  ```
  nm <- as.vector(t(outer(rownames(B), colnames(B), paste, sep = ":")))
  ```
- Line 714: lname, name
  ```
  b  <- setNames(as.vector(t(B)), nm)[colnames(V)]
  ```
- Line 715: name
  ```
  se <- sqrt(diag(V))[names(b)]
  ```
- Line 717: name
  ```
  idx <- startsWith(names(b), paste0(k, ":"))
  ```
- Line 718: name
  ```
  keep <- sub("^-?1:", "", names(b)[idx])
  ```
- Line 719: name
  ```
  list(b = setNames(b[idx], keep), se = setNames(se[idx], keep),
  ```
- Line 731: lat
  ```
  # LaTeX
  ```
- Line 732: name
  ```
  # Rows: a regular expression for the coefficient name, and the label printed.
  ```
- Line 733: name
  ```
  # Patterns rather than exact names, so that Siblings, Topic and howHard5 can be
  ```
- Line 737: gender
  ```
  "^gender"                 = "\\textit{Male}",
  ```
- Line 746: name
  ```
  term_of <- function(col, key) {       # the coefficient name behind each row
  ```
- Line 747: name
  ```
  hit <- grep(key, names(col$b), perl = TRUE, value = TRUE)
  ```
- Line 775: name
  ```
  for (key in names(rows)) {
  ```
- Line 788: son
  ```
  "Age in months in the Poisson columns and in years in the multinomial columns. ",
  ```
- Line 831: lname, name
  ```
  colnames(Perso)<-c("Grade","mean","Trait")
  ```
- Line 868: lname, name
  ```
  colnames(table)<-c("Score","Grade","Percentage")
  ```
- Line 895: name
  ```
  theme_minimal()+theme(axis.ticks.x=element_blank())+scale_fill_manual(values=c("#9E0142","#D53E4F","
  ```
- Line 931: lname, name
  ```
  Y <- sapply(colnames(P), function(k) as.numeric(Y == k))
  ```
- Line 932: name
  ```
  cls <- rownames(coef(x))
  ```
- Line 934: lname, name
  ```
  colnames(S) <- as.vector(t(outer(cls, colnames(X), paste, sep = ":")))
  ```
- Line 947: loc
  ```
  d <- d[d$Age < 225 & (d$StartAlloc == 62 | (d$ToWinner1 != 0 & d$ToWinner2 != 0)), ]
  ```
- Line 952: name
  ```
  for (t in names(traits)) {
  ```
- Line 962: loc
  ```
  d$choice1 <- relevel(factor(choice(d$StartAlloc, d$ToWinner1)), ref = "Equit")
  ```
- Line 963: loc
  ```
  d$choice2 <- relevel(factor(choice(d$StartAlloc, d$ToWinner2)), ref = "Equit")
  ```
- Line 964: loc
  ```
  d$redistribution <- as.numeric(d$StartAlloc == 62)
  ```
- Line 967: gender
  ```
  rhs <- paste("AgeY + I(AgeY^2) + gender + Siblings + Topic +",
  ```
- Line 968: name
  ```
  paste(paste0(names(traits), "_r"), collapse = " + "),
  ```
- Line 976: name
  ```
  cl <- d[rownames(mf), cluster_vars, drop = FALSE]
  ```
- Line 979: lname, name
  ```
  nm <- as.vector(t(outer(rownames(B), colnames(B), paste, sep = ":")))
  ```
- Line 980: lname, name
  ```
  b  <- setNames(as.vector(t(B)), nm)[colnames(V)]
  ```
- Line 981: name
  ```
  se <- sqrt(diag(V))[names(b)]
  ```
- Line 983: name
  ```
  idx  <- startsWith(names(b), paste0(k, ":"))
  ```
- Line 984: name
  ```
  keep <- sub("^[^:]+:", "", names(b)[idx])
  ```
- Line 985: name
  ```
  list(b = setNames(b[idx], keep), se = setNames(se[idx], keep), n = nrow(mf), aic = AIC(m))
  ```
- Line 990: lat
  ```
  # LaTeX
  ```
- Line 993: gender
  ```
  "^gender"                = "\\textit{Male}",
  ```
- Line 1007: name
  ```
  hit <- grep(key, names(col$b), perl = TRUE, value = TRUE)
  ```
- Line 1032: name
  ```
  for (key in names(rows)) {
  ```
- Line 1050: son
  ```
  "\\caption{Multinomial regressions of meritocratic and compensatory initial and final choices: the e
  ```
- Line 1065: lat, school
  ```
  desired_order <- c("Early Elem.", "Late Elem.", "Early Middle", "Late Middle","High School")  # Modi
  ```
- Line 1074: name
  ```
  if (target_category %in% rownames(tab)) {
  ```
- Line 1078: lname, name
  ```
  colnames(selected_row) <- colnames(tab)
  ```
- Line 1083: name
  ```
  selected_row$Variable <- variable_label  # Assign readable variable name
  ```
- Line 1085: loc
  ```
  relocate(Variable, .before = everything())  # Move `Variable` to the first column
  ```
- Line 1091: gender
  ```
  gender_summary <- categorical_summary(data, "gender", "grade2", "M","% Male")
  ```
- Line 1101: second
  ```
  # Convert the matrix in the second column to separate columns
  ```
- Line 1104: name
  ```
  # Rename columns
  ```
- Line 1105: lname, name
  ```
  colnames(summary_df) <- c(grade_column, "mean", "sd")
  ```
- Line 1114: name
  ```
  pivot_wider(names_from = grade_column, values_from = stat)
  ```
- Line 1122: loc
  ```
  relocate(Variable)
  ```
- Line 1127: loc
  ```
  test<-subset(data,(StartAlloc=="62")|(StartAlloc=="31"& ToWinner2 !=0 & ToWinner1 !=0))
  ```
- Line 1129: name
  ```
  # Compute numerical summaries with custom variable names
  ```
- Line 1141: gender
  ```
  gender_summary, siblings_summary, topic_summary)
  ```
- Line 1153: name
  ```
  # Remove row names (index column) without affecting `Variable`
  ```
- Line 1154: name
  ```
  rownames(final_table) <- NULL  # This removes the printed index column
  ```
- Line 1156: name
  ```
  # Rename "Variable" as row names for readability
  ```
- Line 1157: name
  ```
  rownames(final_table) <- final_table$Variable
  ```
- Line 1160: lat
  ```
  # Export as LaTeX
  ```
- Line 1161: lat
  ```
  latex_table <- xtable(final_table, caption = "Summary Statistics by Age Group - mean (standard devia
  ```
- Line 1172: loc
  ```
  df1 <- subset(data, Age < 225 & (StartAlloc == 62 | (StartAlloc == 31 & ToWinner1 != 0)))
  ```
- Line 1173: loc
  ```
  df2 <- subset(data, Age < 225 & (StartAlloc == 62 | (StartAlloc == 31 & ToWinner2 != 0)))
  ```
- Line 1174: loc
  ```
  df1$redist <- as.numeric(df1$StartAlloc == 62)
  ```
- Line 1175: loc
  ```
  df2$redist <- as.numeric(df2$StartAlloc == 62)
  ```
- Line 1178: gender
  ```
  # (1) treatment-by-gender interactions; (2) full treatment-by-environment-by-gender interactions
  ```
- Line 1180: gender
  ```
  "Age + I(Age^2) + Treatment * gender + redist + Siblings + Topic",
  ```
- Line 1181: gender
  ```
  "Age + I(Age^2) + Treatment * redist * gender + Siblings + Topic"
  ```
- Line 1196: gender
  ```
  "^gender"                            = "\\textit{Male}",
  ```
- Line 1201: gender
  ```
  "^Treatmentquestions:gender"         = "\\textit{Talent}$\\times$\\textit{Male}",
  ```
- Line 1202: gender
  ```
  "^Treatmentsliders:gender"           = "\\textit{Effort}$\\times$\\textit{Male}",
  ```
- Line 1203: gender
  ```
  "^redist:gender"                     = "\\textit{Redistribution}$\\times$\\textit{Male}",
  ```
- Line 1204: gender
  ```
  "^Treatmentquestions:redist:gender"  = "\\textit{Talent}$\\times$\\textit{Redistribution}$\\times$\\
  ```
- Line 1205: gender
  ```
  "^Treatmentsliders:redist:gender"    = "\\textit{Effort}$\\times$\\textit{Redistribution}$\\times$\\
  ```
- Line 1211: name
  ```
  old <- rownames(ct)
  ```
- Line 1213: name
  ```
  for (p in names(labels)) new[grepl(p, old)] <- labels[[p]]
  ```
- Line 1216: name
  ```
  coef.names  = new,
  ```
- Line 1217: name
  ```
  coef        = unname(ct[, "Estimate"]),
  ```
- Line 1218: name
  ```
  se          = unname(ct[, "Std. Error"]),
  ```
- Line 1219: name
  ```
  pvalues     = unname(ct[, "Pr(>|t|)"]),
  ```
- Line 1220: name
  ```
  gof.names   = c("Num. obs.", "R$^2$", "Adj. R$^2$"),
  ```
- Line 1221: name
  ```
  gof         = c(nobs(m), unname(r2(m, "r2")), unname(r2(m, "ar2"))),
  ```
- Line 1239: name
  ```
  custom.model.names = c("Initial", "Initial", "Final", "Final"),
  ```
- Line 1240: name
  ```
  custom.coef.map    = as.list(setNames(unname(labels), unname(labels))),
  ```
- Line 1249: gender, loc, location
  ```
  caption            = "Gender effects in the \\textit{initial} and \\textit{final} allocations to the
  ```
- Line 1251: gender
  ```
  label              = "regtreatmentGender",
  ```
- Line 1267: lat
  ```
  # Row labels, in the order of the table. Later patterns override earlier ones.
  ```
- Line 1273: gender
  ```
  "^gender"                                            = "\\textit{Male}",
  ```
- Line 1276: loc
  ```
  "^as\\.factor\\(StartAlloc\\)62$"                    = "\\textit{Redistribution}",
  ```
- Line 1277: loc
  ```
  "^Age:as\\.factor\\(StartAlloc\\)62$|^as\\.factor\\(StartAlloc\\)62:Age$" =
  ```
- Line 1279: loc
  ```
  "StartAlloc.*Age\\^2|Age\\^2.*StartAlloc"            = "\\textit{Age}$^2\\times$\\textit{Redistribut
  ```
- Line 1285: name
  ```
  old <- rownames(ct)
  ```
- Line 1287: name
  ```
  for (p in names(labels)) new[grepl(p, old)] <- labels[[p]]
  ```
- Line 1289: name
  ```
  coef.names  = new,
  ```
- Line 1290: name
  ```
  coef        = unname(ct[, "Estimate"]),
  ```
- Line 1291: name
  ```
  se          = unname(ct[, "Std. Error"]),
  ```
- Line 1292: name
  ```
  pvalues     = unname(ct[, "Pr(>|t|)"]),
  ```
- Line 1293: name
  ```
  gof.names   = c("Num. obs.", "R$^2$", "Adj. R$^2$"),
  ```
- Line 1294: name
  ```
  gof         = c(nobs(m), unname(r2(m, "r2")), unname(r2(m, "ar2"))),
  ```
- Line 1303: loc
  ```
  d62  <- data[data$Age < 225 & data$StartAlloc == 62, ]
  ```
- Line 1304: loc
  ```
  d31  <- data[data$Age < 225 & data$StartAlloc == 31 & rec, ]
  ```
- Line 1308: gender
  ```
  ctrl <- "Treatment + gender + Siblings + Topic"
  ```
- Line 1315: loc
  ```
  list("Age * as.factor(StartAlloc)",                                     dall),
  ```
- Line 1316: loc
  ```
  list("Age * as.factor(StartAlloc) + I(Age^2) * as.factor(StartAlloc)",  dall)
  ```
- Line 1323: name
  ```
  custom.model.names = c("Redistribution", "Redistribution", "Addition", "Addition", "All", "All"),
  ```
- Line 1324: name
  ```
  custom.coef.map    = as.list(setNames(unname(labels), unname(labels))),
  ```
- Line 1332: loc, location
  ```
  caption            = paste0("\\textit{", when, "} allocation to the loser by treatments and age with
  ```
- Line 1357: lat
  ```
  data$grade2 <- factor(data$grade2, levels = c("Early Elem.", "Late Elem.", "Early Middle",
  ```
- Line 1358: lat, school
  ```
  "Late Middle", "High School"))
  ```
- Line 1361: lat
  ```
  "^grade2.*Late Elem"    = "\\textit{Late Elem.}",
  ```
- Line 1363: lat
  ```
  "^grade2.*Late Mid"     = "\\textit{Late Middle}",
  ```
- Line 1364: school
  ```
  "^grade2.*High"         = "\\textit{High School}",
  ```
- Line 1367: gender
  ```
  "^gender"               = "\\textit{Male}",
  ```
- Line 1375: name
  ```
  old <- rownames(ct)
  ```
- Line 1377: name
  ```
  for (p in names(labels)) new[grepl(p, old)] <- labels[[p]]
  ```
- Line 1379: name
  ```
  coef.names  = new,
  ```
- Line 1380: name
  ```
  coef        = unname(ct[, "Estimate"]),
  ```
- Line 1381: name
  ```
  se          = unname(ct[, "Std. Error"]),
  ```
- Line 1382: name
  ```
  pvalues     = unname(ct[, "Pr(>|t|)"]),
  ```
- Line 1383: name
  ```
  gof.names   = c("Num. obs.", "R$^2$", "Adj. R$^2$"),
  ```
- Line 1384: name
  ```
  gof         = c(nobs(m), unname(r2(m, "r2")), unname(r2(m, "ar2"))),
  ```
- Line 1390: gender
  ```
  rhs <- "grade2 + Treatment + gender + Siblings + Topic"
  ```
- Line 1394: loc
  ```
  d <- if (env == 62) data[data$Age < 225 & data$StartAlloc == 62, ] else
  ```
- Line 1395: loc
  ```
  data[data$Age < 225 & data$StartAlloc == 31 & rec, ]
  ```
- Line 1403: name
  ```
  custom.model.names = c("Redistribution", "Addition", "Redistribution", "Addition"),
  ```
- Line 1404: name
  ```
  custom.coef.map    = as.list(setNames(unname(labels), unname(labels))),
  ```
- Line 1436: loc, location
  ```
  # Appendix B5 (redistribution) and B6 (addition): final allocation regressed on
  ```
- Line 1441: name
  ```
  # Rows: pattern for the coefficient name, printed label, decimals
  ```
- Line 1445: gender
  ```
  list("^gender",               "Male",      3),
  ```
- Line 1454: name
  ```
  hit <- grep(pattern, rownames(ct), perl = TRUE)
  ```
- Line 1461: name
  ```
  envname <- if (env == 62) "redistribution" else "addition"
  ```
- Line 1462: loc
  ```
  d <- if (env == 62) data[data$Age < 225 & data$StartAlloc == 62, ] else
  ```
- Line 1463: loc
  ```
  data[data$Age < 225 & data$StartAlloc == 31 & data$ToWinner2 != 0, ]
  ```
- Line 1468: gender
  ```
  fits[[length(fits) + 1]] <- feols(8 - PayWinner2 ~ Age + I(Age^2) + gender + Siblings + Topic, data 
  ```
- Line 1520: name
  ```
  scale_color_manual(values = c("Luck" = "grey", "Effort" = "dodgerblue", "Talent" = "gold"), name = "
  ```
- Line 1531: loc, location
  ```
  "OLS regressions of \\textit{final} allocation in the \\textit{redistribution} treatment, performed 
  ```
- Line 1536: loc, location
  ```
  "OLS regressions of \\textit{final} allocation in the \\textit{addition} treatment, performed separa
  ```
- Line 1542: gender
  ```
  # Needs in `data`: Tom1..Tom16 (answer, asterisk = correct), scoreTom, grade1 (1..12), gender (M/F),
  ```
- Line 1554: lat
  ```
  # Grades 1 to 5, and 5 to 12: change in the mean and correlation with age
  ```
- Line 1561: name
  ```
  PCC        = round(unname(ct$estimate), 2),
  ```
- Line 1576: name
  ```
  names(pct) <- emotion
  ```
- Line 1586: name
  ```
  rownames(clarity) <- paste(1:16, emotion)
  ```
- Line 1590: gender
  ```
  # Gender
  ```
- Line 1591: gender
  ```
  tt <- t.test(scoreTom ~ gender, data = d[d$gender %in% c("F", "M"), ])
  ```
- Line 1604: child
  ```
  # Mini-IPIP: the frame that holds the items (the older children only) and the
  ```
- Line 1605: name
  ```
  # item names, in the order administered. `data_ipip` is `data` itself when the
  ```
- Line 1606: name
  ```
  # items are columns of `data`; otherwise name the frame that has them.
  ```
- Line 1614: name
  ```
  missing <- setdiff(ipip_items, names(data_ipip))
  ```
- Line 1622: name
  ```
  names(correct) <- make.names(emotion)
  ```
- Line 1627: school
  ```
  # High schoolers: percent correct by image
  ```
- Line 1629: school
  ```
  cat("\nHigh school (grades 11-12), percent correct by image:\n"); print(round(hs, 0))
  ```
- Line 1630: name
  ```
  cat("Below 70%:", paste0(names(hs)[hs < 70], " (", round(hs[hs < 70], 0), "%)", collapse = ", "), "\
  ```
- Line 1634: lat
  ```
  # Reliability: Cronbach's alpha on tetrachoric correlations, by age group
  ```
- Line 1636: lat, school
  ```
  labels = c("Early elem.", "Late elem.", "Early middle", "Late middle", "High school"))
  ```
- Line 1645: lat
  ```
  # Exploratory factor analysis: three factors on tetrachoric correlations
  ```
- Line 1651: name
  ```
  for (k in 1:3) cat("Factor", k, ":", paste(rownames(L)[assign_f == k], collapse = ", "), "\n")
  ```
- Line 1655: name
  ```
  paste0("F", k, " =~ ", paste(rownames(L)[assign_f == k], collapse = " + "))), collapse = "\n")
  ```
- Line 1657: name
  ```
  fit <- lavaan::cfa(model, data = sub, ordered = names(sub), std.lv = TRUE)
  ```
- Line 1673: name
  ```
  c(r = round(unname(ct$estimate), 2), p = signif(ct$p.value, 2))
  ```
- Line 1682: gender
  ```
  # BigN, BigO, Age (months), grade1 (1..12), gender, ClientID; and
  ```
- Line 1686: name
  ```
  trait_name <- c(O = "Openness", C = "Conscientiousness", E = "Extraversion",
  ```
- Line 1699: lat
  ```
  cat("\nCorrelation between score and age (months):\n")
  ```
- Line 1702: name
  ```
  c(PCC = round(unname(ct$estimate), 2), p = signif(ct$p.value, 2))
  ```
- Line 1711: gender
  ```
  m$Male <- as.numeric(m$gender == "M")
  ```
- Line 1713: name
  ```
  for (t in names(ipip)) {
  ```
- Line 1722: name
  ```
  fits <- lapply(names(traits), function(t)
  ```
- Line 1724: name
  ```
  names(fits) <- names(traits)
  ```
- Line 1729: name
  ```
  if (!term %in% rownames(ct)) return(c("", ""))
  ```
- Line 1738: name
  ```
  paste(" &", paste("Pict", names(traits), collapse = " & "), "\\\\"), "\\hline")
  ```
- Line 1739: name
  ```
  for (t in names(traits)) t18 <- c(t18, row2(paste("mini-IPIP", t), paste0("ipip", t)))
  ```
- Line 1751: lat
  ```
  # Table 19: correlation of each P-Big 5 score with each mini-IPIP item -------
  ```
- Line 1753: block, loc
  ```
  block <- function(t) {
  ```
- Line 1762: block, loc, name
  ```
  blocks <- lapply(names(traits), block)
  ```
- Line 1763: block, loc, lon
  ```
  body <- unlist(lapply(seq_along(blocks), function(i) {
  ```
- Line 1764: block, loc
  ```
  b <- blocks[[i]]; if (i < length(blocks)) b[length(b)] <- paste(b[length(b)], "&"); b
  ```
- Line 1769: lat
  ```
  "\\caption{\\small Correlations between P-Big 5 scores and IPIP scores by question. * indicates IPIP
  ```
- Line 1774: name
  ```
  for (t in names(traits)) for (q in ipip[[t]]) {
  ```
- Line 1786: second
  ```
  # full trait-by-environment-by-condition interactions (second model).
  ```
- Line 1787: lon
  ```
  # Same sample, residuals and clustering as Table 6. Output uses longtable.
  ```
- Line 1794: lname, name
  ```
  Y <- sapply(colnames(P), function(k) as.numeric(Y == k))
  ```
- Line 1795: name
  ```
  cls <- rownames(coef(x))
  ```
- Line 1797: lname, name
  ```
  colnames(S) <- as.vector(t(outer(cls, colnames(X), paste, sep = ":")))
  ```
- Line 1810: loc
  ```
  d <- d[d$Age < 225 & (d$StartAlloc == 62 | (d$ToWinner1 != 0 & d$ToWinner2 != 0)), ]
  ```
- Line 1813: name
  ```
  for (t in names(traits)) {
  ```
- Line 1821: loc
  ```
  d$choice1 <- relevel(factor(choice(d$StartAlloc, d$ToWinner1)), ref = "Equit")
  ```
- Line 1822: loc
  ```
  d$choice2 <- relevel(factor(choice(d$StartAlloc, d$ToWinner2)), ref = "Equit")
  ```
- Line 1823: loc
  ```
  d$redistribution <- as.numeric(d$StartAlloc == 62)
  ```
- Line 1826: name
  ```
  tr   <- paste0(names(traits), "_r")
  ```
- Line 1827: gender
  ```
  base <- paste("AgeY + I(AgeY^2) + gender + Siblings + Topic +", paste(tr, collapse = " + "),
  ```
- Line 1838: name
  ```
  cl <- d[rownames(mf), cluster_vars, drop = FALSE]
  ```
- Line 1841: lname, name
  ```
  nm <- as.vector(t(outer(rownames(B), colnames(B), paste, sep = ":")))
  ```
- Line 1842: lname, name
  ```
  b  <- setNames(as.vector(t(B)), nm)[colnames(V)]
  ```
- Line 1843: name
  ```
  se <- sqrt(diag(V))[names(b)]
  ```
- Line 1845: name
  ```
  idx  <- startsWith(names(b), paste0(k, ":"))
  ```
- Line 1846: name
  ```
  keep <- sub("^[^:]+:", "", names(b)[idx])
  ```
- Line 1847: name
  ```
  list(b = setNames(b[idx], keep), se = setNames(se[idx], keep), n = nrow(mf), aic = AIC(m))
  ```
- Line 1855: gender
  ```
  "^gender" = it("Male"), "^Siblings" = it("Siblings"), "^Topic" = it("STEM"))
  ```
- Line 1856: name
  ```
  for (t in names(traits)) rows[paste0("^", t, "_r$")] <- paste0(t, " (resid)")
  ```
- Line 1860: name
  ```
  for (t in names(traits)) rows[paste0("^", t, "_r:redistribution$")] <- paste0(it(t), X, it("redistri
  ```
- Line 1861: name
  ```
  for (t in names(traits)) {
  ```
- Line 1867: name
  ```
  for (t in names(traits)) {
  ```
- Line 1874: name
  ```
  hit <- grep(key, names(col$b), perl = TRUE, value = TRUE)
  ```
- Line 1887: lon
  ```
  # longtable
  ```
- Line 1904: lon
  ```
  "\\begin{longtable}{l cc cc}",
  ```
- Line 1916: name
  ```
  for (key in names(rows)) {
  ```
- Line 1927: lon
  ```
  "\\end{longtable}",
  ```
- Line 1953: lname, name
  ```
  Y <- sapply(colnames(P), function(k) as.numeric(Y == k))
  ```
- Line 1954: name
  ```
  cls <- rownames(coef(x))                       # non-baseline classes
  ```
- Line 1956: lname, name
  ```
  colnames(S) <- as.vector(t(outer(cls, colnames(X), paste, sep = ":")))
  ```
- Line 1969: son
  ```
  # in the Poisson columns as in the original code
  ```
- Line 1983: loc
  ```
  base62 <- with(data, Age < 225 & Treatment != "luck" & StartAlloc == 62)
  ```
- Line 1984: loc
  ```
  base31 <- with(data, Age < 225 & Treatment != "luck" & StartAlloc == 31 &
  ```
- Line 1988: gender
  ```
  ctrl   <- "gender + Siblings + Topic + Treatment + howHard5 + howWell5 + scoreTom + BigE + BigA + Bi
  ```
- Line 1991: son
  ```
  rhs_p  <- if (age_unit == "years") rhs_y else rhs_m   # Poisson columns
  ```
- Line 1993: son
  ```
  # Poisson column: coefficients, two-way clustered SE (session, campus)
  ```
- Line 1995: son
  ```
  m <- glm(as.formula(paste(lhs, "~", rhs_p)), family = poisson, data = d)
  ```
- Line 2006: name
  ```
  cl <- d[rownames(mf), cluster_vars, drop = FALSE]
  ```
- Line 2009: lname, name
  ```
  nm <- as.vector(t(outer(rownames(B), colnames(B), paste, sep = ":")))
  ```
- Line 2010: lname, name
  ```
  b  <- setNames(as.vector(t(B)), nm)[colnames(V)]
  ```
- Line 2011: name
  ```
  se <- sqrt(diag(V))[names(b)]
  ```
- Line 2013: name
  ```
  idx <- startsWith(names(b), paste0(k, ":"))
  ```
- Line 2014: name
  ```
  keep <- sub("^-?1:", "", names(b)[idx])
  ```
- Line 2015: name
  ```
  list(b = setNames(b[idx], keep), se = setNames(se[idx], keep),
  ```
- Line 2027: lat
  ```
  # LaTeX
  ```
- Line 2028: name
  ```
  # Rows: a regular expression for the coefficient name, and the label printed.
  ```
- Line 2029: name
  ```
  # Patterns rather than exact names, so that Siblings, Topic and howHard5 can be
  ```
- Line 2033: gender
  ```
  "^gender"                 = "\\textit{Male}",
  ```
- Line 2048: name
  ```
  term_of <- function(col, key) {       # the coefficient name behind each row
  ```
- Line 2049: name
  ```
  hit <- grep(key, names(col$b), perl = TRUE, value = TRUE)
  ```
- Line 2077: name
  ```
  for (key in names(rows)) {
  ```
- Line 2090: son
  ```
  "Age in months in the Poisson columns and in years in the multinomial columns. ",
  ```

**/replication-package/Replication Package/Paper/Figs/Table16.tex**

- Line 26: loc, location
  ```
  \caption{OLS regressions of \textit{final} allocation in the \textit{redistribution} treatment, perf
  ```

**/replication-package/Replication Package/Paper/Figs/Table17.tex**

- Line 26: loc, location
  ```
  \caption{OLS regressions of \textit{final} allocation in the \textit{addition} treatment, performed 
  ```

**/replication-package/Replication Package/Paper/Figs/Table2.tex**

- Line 42: loc, location
  ```
  \caption{Main treatment effects in the \textit{initial} and \textit{final} allocation to the loser.}
  ```

**/replication-package/Replication Package/Paper/Figs/Table20.tex**

- Line 2: lon
  ```
  \begin{longtable}{l cc cc}
  ```
- Line 122: lon
  ```
  \end{longtable}
  ```

**/replication-package/Replication Package/Paper/Figs/Table21.tex**

- Line 2: lon
  ```
  \begin{longtable}{l cc cc}
  ```
- Line 122: lon
  ```
  \end{longtable}
  ```

**/replication-package/Replication Package/Paper/Figs/Table3.tex**

- Line 39: loc, location
  ```
  \caption{\textit{Initial} allocation to the loser by treatments and age}
  ```

**/replication-package/Replication Package/Paper/Figs/Table4.tex**

- Line 39: loc, location
  ```
  \caption{\textit{Final} allocation to the loser by treatments and age}
  ```

**/replication-package/Replication Package/Paper/Figs/summary_table.tex**

- Line 1: lat
  ```
  % latex table generated in R 4.4.2 by xtable 1.8-4 package
  ```
- Line 7: lat, school
  ```
  & Early Elem. & Late Elem. & Early Middle & Late Middle & High School \\
  ```

**/replication-package/Replication Package/Paper/Figs/table10.tex**

- Line 39: loc, location
  ```
  \caption{\textit{Initial} allocation to the loser by treatments and age with clustered standard erro
  ```

**/replication-package/Replication Package/Paper/Figs/table11.tex**

- Line 39: loc, location
  ```
  \caption{\textit{Initial} allocation to the loser by treatments and age with clustered standard erro
  ```

**/replication-package/Replication Package/Paper/Figs/table12.tex**

- Line 39: loc, location
  ```
  \caption{\textit{Final} allocation to the loser by treatments and age with clustered standard errors
  ```

**/replication-package/Replication Package/Paper/Figs/table13.tex**

- Line 39: loc, location
  ```
  \caption{\textit{Final} allocation to the loser by treatments and age with clustered standard errors
  ```

**/replication-package/Replication Package/Paper/Figs/table14.tex**

- Line 11: lat
  ```
  \textit{Late Elem.}   & $-0.012$      & $0.110$        & $-0.023$       & $0.185^{*}$    \\
  ```
- Line 15: lat
  ```
  \textit{Late Middle}  & $-0.062$      & $0.182^{*}$    & $-0.047$       & $0.248^{**}$   \\
  ```
- Line 17: school
  ```
  \textit{High School}  & $-0.058$      & $0.141$        & $0.064$        & $0.128$        \\
  ```

**/replication-package/Replication Package/Paper/Figs/table15.tex**

- Line 11: lat
  ```
  \textit{Late Elem.}   & $0.002$       & $0.097$        & $0.015$        & $0.184^{*}$    \\
  ```
- Line 15: lat
  ```
  \textit{Late Middle}  & $-0.053$      & $0.171^{*}$    & $0.006$        & $0.251^{**}$   \\
  ```
- Line 17: school
  ```
  \textit{High School}  & $-0.074$      & $0.168$        & $0.051$        & $0.157$        \\
  ```

**/replication-package/Replication Package/Paper/Figs/table19.tex**

- Line 59: lat
  ```
  \caption{\small Correlations between P-Big 5 scores and IPIP scores by question. * indicates IPIP qu
  ```

**/replication-package/Replication Package/Paper/Figs/table6.tex**

- Line 50: son
  ```
  \caption{Multinomial regressions of meritocratic and compensatory initial and final choices: the eff
  ```

**/replication-package/Replication Package/Paper/Figs/table9.tex**

- Line 51: gender, loc, location
  ```
  \caption{Gender effects in the \textit{initial} and \textit{final} allocations to the loser.}
  ```
- Line 52: gender
  ```
  \label{regtreatmentGender}
  ```

**/replication-package/Replication Package/Paper/revised ms.tex**

- Line 15: name
  ```
  \usepackage[dvipsnames]{xcolor}
  ```
- Line 19: url
  ```
  \usepackage{url}
  ```
- Line 29: url
  ```
  %\usepackage[pdfborder={0 0 0}, bookmarksnumbered=true, bookmarksopenlevel=1, colorlinks=true, linkc
  ```
- Line 36: lat
  ```
  \usepackage{latexsym}
  ```
- Line 42: url
  ```
  \usepackage[pdfborder={0 0 0}, bookmarksnumbered=true, bookmarksopenlevel=1, colorlinks=true, linkco
  ```
- Line 44: name
  ```
  \usepackage[dvipsnames]{xcolor}
  ```
- Line 45: lon
  ```
  \usepackage{longtable}
  ```
- Line 96: school
  ```
  \centerline{\Large {\bf Developmental Meritocracy}  \footnote{We thank the members of the Los Angele
  ```
- Line 128: city, gender, lat, loc, location, son
  ```
  Pooled estimates also indicate lower transfers to the loser when the winner is selected by talent ra
  ```
- Line 156: child, lat
  ```
  A pioneering study by \citet{Fehr2008} examined the choices of children aged 3 to 8 in three binary 
  ```
- Line 157: child
  ```
  In \citet{almaas2010fairness}, children aged 10 to 18 first completed a production task in which ear
  ```
- Line 165: gender, son
  ```
  Overall, as we develop below, in this paper we systematically analyze redistributive preferences by 
  ```
- Line 183: loc, location, son
  ```
  The paper is organized as follows. In section \ref{sec-design}, we present the experimental design. 
  ```
- Line 187: address, child, loc
  ```
  We recruited children and adolescents to study the decision of an impartial observer who allocates r
  ```
- Line 189: second, son
  ```
  \emph{Experiment}. The experiment consists of two games programmed in `oTree' \citep{chen2016otree}.
  ```
- Line 192: loc
  ```
  \emph{Timing}. We first informed participants that they all would play an ``observer task" followed 
  ```
- Line 193: second, son
  ```
  with clear emphasis that no further modifications would be possible afterwards. These tasks were fol
  ```
- Line 196: loc, location
  ```
  \emph{Observer task}. The impartial observer game used a visually intuitive interface (see Figure \r
  ```
- Line 212: loc
  ```
  \caption{\emph{Addition}: 4 tokens (bottom) must be allocated between winner and loser (with at leas
  ```
- Line 221: second
  ```
  In the \emph{effort\/} task, participants were randomly and anonymously paired to compete in an effo
  ```
- Line 232: second
  ```
  \caption{\emph{Effort}: participants had 90 seconds to position as many sliders as possible at 50\la
  ```
- Line 244: loc, location
  ```
  Overall, the experiment consists of six variants, following a $3\times 2 $ between-subject design: t
  ```
- Line 247: lat
  ```
  \emph{Population}.
  ```
- Line 267: lat
  ```
  \centering\caption{Number of participants by grade, treatment, and condition} \label{table-populatio
  ```
- Line 271: school
  ```
  We identified a payment method that was uniform across all ages and highly valued by participants. A
  ```
- Line 275: child
  ```
  We therefore created an alternative RMET task, called DeRMET (Developmental RMET), specifically for 
  ```
- Line 288: son
  ```
  \includegraphics[height=2.0in]{Figs/personality4.png}
  ```
- Line 296: social, son
  ```
  \emph{Pictorial Big Five (P-Big 5)}. Next, we performed a novel version of the Big Five questionnair
  ```
- Line 297: child, lat, son
  ```
  mccrae1987validation, goldberg1993structure}. Studies have employed a wide array of verbal questionn
  ```
- Line 299: address, child
  ```
  To address these challenges and ensure consistent testing across individuals aged 6 to 18, we again 
  ```
- Line 308: birth, gender, loc, location, school
  ```
  We chose this timing intentionally to mitigate any potential demand effect that might prompt partici
  ```
- Line 330: lat, loc, location
  ```
  As it is well-known, when the observer is solely concerned with the participants' final utilities ($
  ```
- Line 344: loc, location, son
  ```
  Importantly, our framework is designed for impartial third-party judgments without personal stakes. 
  ```
- Line 351: child, son
  ```
  Although the overall sample is large for an in-person experiment with children, the six treatments c
  ```
- Line 368: lat, loc, location
  ```
  We expected that allocations to the loser would be lowest under \emph{talent}, intermediate under \e
  ```
- Line 403: child, gender, lat
  ```
  Consistent with the literature on inequality acceptance in adults \citep{almaas2020cutthroat}, we ob
  ```

