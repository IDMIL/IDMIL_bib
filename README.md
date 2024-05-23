# Rubric for IDMIL Bibliography Formation:

## 1. Adding New Conference or Journal Names:

- **Step 1**: Identify the official full name of the new conference or journal.
- **Step 2**: Use an abbreviation (acronym) for the conference or journal name. Use uppercase letters and ensure that it is short, memorable, and as close to the commonly used acronym as possible.
- **Step 3**: Add the new conference or journal to the BibTeX file using the `@string` directive. Format the entry to match the existing examples:
  - Use `@string{ACRONYM = "Full Name of the Conference or Journal"}`.
  - Ensure that the full name of conference proceedings starts with "Proceedings of the" for consistency.
  - For journals, use curly braces `{}` if the title has special formatting needs; otherwise, use quotation marks `""`.
- **Step 4**: Place the new `@string` entry in the appropriate category.

## Example:
```bibtex
@string{ACRONYM = "Proceedings of the New Example Conference"}
```

## 2. Adding New References:

- **Step 1**: Determine the type of reference you are adding (e.g., conference paper, journal article). Use `@inproceedings` for conference papers and `@article` for journal articles.
- **Step 2**: Construct the citation key for the new reference. Use the format "lastNameYearKeyword":
  - "lastName" is the last name of the first author.
  - "Year" is the four-digit publication year.
  - "Keyword" is a short, descriptive keyword from the title.
- **Step 3**: Fill in the reference details following the BibTeX format:
  - Use commas to separate each field within an entry.
  - Wrap the title of the work in double braces `{{}}` to preserve the case of the title.
  - List all authors in the format "Last, First and Last, First", using "and" between authors.
  - Specify the `booktitle` or `journal` field using the acronym defined by the `@string` directive.
  - Include page numbers, volume, number, and other relevant details as applicable.
- **Step 4**: Ensure that the reference adheres to formatting conventions, including the use of braces and quotation marks.
- **Step 5**: Place the new reference in the bibliography file, keeping the references within each category in alphabetical order based on the citation key.

## Example:
```bibtex
@inproceedings{Naef2006VR,
	title        = {{A VR Interface for Collaborative 3D Audio Performance}},
	author       = {Naef, Martin and Collicott, Daniel},
	booktitle    = NIME,
	pages        = {57--60}
	year         = 2006
}
@article{ Waters2021Entanglements,
	 title = {{The entanglements which make instruments musical: Rediscovering sociality}},
	 author = { Waters, Simon },
	 journal = JNMR,
	 volume = { 50 },
	 number = { 2 },
	 pages = { 133--146 },
	 year = { 2021 }
}

@book{ Calegario2019Springer,
	 title = {{Designing Digital Musical Instruments Using Probatio: A Physical Prototyping Toolkit }},
	 author = { Calegario, Filipe },
	 publisher = { Springer Cham },
	 address = { Cham, Switzerland },
	 year = { 2019 }
}
@incollection{ Hardjowirogo2017Instrumentality,
	 title = {{ Instrumentality. On the Construction of Instrumental Identity }},
	 author = { Hardjowirogo, Sarah-Indriyati },
	 booktitle = { Musical Instruments in the 21st Century: Identities, Configurations, Practices },
	 pages = { 9-24 },
	 publisher = { Springer },
	 address = { Singapore },
	 year = { 2017 }
}
@phdthesis{Adnan2013Thesis,
  title = {{Working Through: Characterising and Evaluating Skill with Digital Musical Interactions}},
  author = {Marquez-Borbon, Adnan},
  school = {Queen's University Belfast},
  address = { Belfast, Northern Ireland },
  year = {2013},
} # Add type = {{PhD Dissertation}}, if you don't want it to appear as a "PhD Thesis" 

@mastersthesis{malloch_consort_2008,
	title = {{A Consort of Gestural Musical Controllers: Design, Construction, and Performance}},
	author = {Malloch, Joseph W},	
	school = {McGill University},
	year = {2008},
} # It will appear as a "Master's Thesis"

```

## General Guidelines:

- **Consistency**: Ensure that all entries in the bibliography file follow the same formatting and naming conventions.
- **Review and Validation**: Regularly review the bibliography for errors, duplications, or inconsistencies. Use a BibTeX validator to assist in finding and fixing issues.
- **Documentation**: Provide clear documentation and examples within the lab's guidelines to help new members understand how to correctly add references.
- **Updates**: Keep the bibliography file up-to-date by adding new references as they are used in lab publications or reports, and by updating existing references if errors are found.
