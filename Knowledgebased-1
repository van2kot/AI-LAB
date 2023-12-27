def evaluate_expression(q, p, r):
    expression_result = (p or q) and (not r or p)
    return expression_result

def generate_truth_table():
    print("\tExpression (KB)")
    print("---|---|---|-----------------|------------")

    for q in [True, False]:
        for p in [True, False]:
            for r in [True, False]:
                expression_result = evaluate_expression(q, p, r)
                query_result = p and r

                print(f"{expression_result}| {query_result}")

def query_entails_knowledge():
    for q in [True, False]:
        for p in [True, False]:
            for r in [True, False]:
                expression_result = evaluate_expression(q, p, r)
                query_result = p and r

                if expression_result and not query_result:
                    return False


    return True

def main():
    generate_truth_table()
    if query_entails_knowledge():
        print("\nQuery entails the knowledge.")
    else:
        print("\nQuery does not entail the knowledge.")

if __name__ == "__main__":
    main()
